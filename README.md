# Marktplaats Scraper

Want to know the average price on [Marktplaats](www.marktplaats.nl) for a product you want to sell? I would!

## Installation

```
git clone git://github.com/manuelvanrijn/mp-scraper.git
cd mp-scraper
npm install
```

## Example

Let's say I want to sell my old iPhone 4. On Marktplaats I'll setup some filters (above 100 EUR, not the 3gs etc.). After you finshed filtering, copy the url.

In this example we'll us the iPhone 4 example [url](http://kopen.marktplaats.nl/telecommunicatie/mobiele-telefoons-apple-iphone/c1953.html?xl=1&ds=to%3A1%3Bpu%3A0%3Bl1%3A820%3Bl2%3A1953%3Bdi%3A%3Bpp%3A0%3Blt%3Azip%3Bsfds%3A1%3Bpt%3A0%3Bmp%3Anumeric%3Bkw%3Aiphone%25204%2520-4s%3Bosi%3A2&ppu=0&aw%5B288%5D%5B0%5D=1629&aw%5B289%5D%5B0%5D=1631&aw%5B3437%5D%5B0%5D=56694&p=1&pmin=100)

```
$ bin/mp-scraper

prompt: Please specify the marktplaats url:  http://kopen.marktplaats.nl/telecommunicatie/mobiele-telefoons-apple-iphone/c1953.html?xl=1&ds=to%3A1%3Bpu%3A0%3Bl1%3A820%3Bl2%3A1953%3Bdi%3A%3Bpp%3A0%3Blt%3Azip%3Bsfds%3A1%3Bpt%3A0%3Bmp%3Anumeric%3Bkw%3Aiph%5B3437%5D%5B0%5D=56694&p=1&pmin=100%5B288%5D%5B0%5D=1629&aw%5B289%5D%5B0%5D=1631&aw
prompt: How many page's do you want to scrap? (leave blank to scrap all pages):

== Marktplaats scraper started ==
* Found: 29 pages to scrape

  scraping [=======================================] 100% 0.0s

  Number of products:  777
  AVG price:           348.76 EUR
  MAX price:           679 EUR
  MIN price:           100 EUR
```

## Prerequisites

You must have node installed on your machine
