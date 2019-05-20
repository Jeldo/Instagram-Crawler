### Instagram Crawler & Sorter

### Install

## Crawler

1. Make sure you have Chrome browser installed.
2. Download [Chromedriver](https://sites.google.com/a/chromium.org/chromedriver/) and put it in current folder.
3. Install Selenium: `pip3 install -r requirements.txt`.

For linux,

1. `wget https://chromedriver.storage.googleapis.com/2.37/chromedriver_linux64.zip`
2. `unzip chromedriver_linux64.zip`
3. `apt-get install chromium-browser`

## Sorter

1. Make sure you have Google Maps Platform API Key in the directory.

### Usage

## Crawler

1. Make sure variable `PATH` is properly assigned in `place_crawler.py`.
2. Enable or disable `headless` in chrome option.
4. Run by `python3 place_crawler.py {number of posts} {number of threads} {hashtag}`
    ex: `python3 place_crawler.py 1000 10`
5. JSON formatted document(including `location`, `link`, `timestamp`,`captions`, `hashtags` respectively) will be created.

## Sorter

1. Make sure to use same `hashtag` that used in the Crawler.
2. `place_{hashtag}_posts.json` should be in the directory.
3. Run by `python3 place_sorter.py {number of threads} {hashtag}`
4. Groupped places will be created in json file.

####

This crawler might not run properly depending on instagram's update.
Argparser will be added soon. 😅

Currently sorter doesn't work properly outside of Korea.
NLP or ML could be applied for solving address problem. 🤔