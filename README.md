# olxscraper
My first scraper with python Scrapy

## install scrapy
	sudo -H pip install Scrapy

## Create project
	scrapy startproject olx
	cd olx/
	scrapy genspider electronics  www.olx.in


## Test scrapy
	scrapy crawl   electronics
	scrapy crawl --nolog  electronics

## Get page info and test
	scrapy shell https://www.olx.in/item/ps3-250gb-with-8-original-games-disc-1-controller-ID1qXSyF.html#506dd58b3b

## Save data in csv or json format
	scrapy crawl  electronics -o data.csv -t csv


### ToDoS
- [x] Simple web crawler
- [ ] Add single proxy
- [ ] Add multiple proxies
- [ ] Deal with captcha