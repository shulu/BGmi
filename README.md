BGmi
====
BGmi is a cli tool for subscribed bangumi.

---

[![Build Status](https://travis-ci.org/RicterZ/BGmi.svg?branch=master)](https://travis-ci.org/RicterZ/BGmi)

---

## Feature

+ Subscribe/Unsubscribe bangumi
+ Bangumi-updating schedule
+ Bangumi episode infomartion
+ HTTP Server for RSS feed (for uTorrent, etc.)

## Installation
For **Mac OS X / Linux**:

    git clone https://github.com/RicterZ/BGmi
    cd BGmi
    python setup.py install

Or use pip:

    pip install bgmi

For **Windows**: BGmi dose not support Windows now.  

## Usage
Show bangumi calendar of this week:

    bgmi cal all

Subscribe bangumi:

    bgmi add "Re：從零開始的異世界生活" "暗殺教室Ⅱ" "線上遊戲的老婆不可能是女生？" "在下坂本，有何貴幹？" "JoJo的奇妙冒險 不滅鑽石"

Unsubscribe bangumi:

    bgmi del --name "暗殺教室Ⅱ"

Update bangumi calendar and episode, and write to download.xml:  

    bgmi update --update

Start a HTTP Server for download.xml:

    bgmi http --port 12345

Add crontab job:

    bgmi crontab --download

