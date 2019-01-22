# olx Spider
My first scraper with python Scrapy

## install scrapy
	sudo -H pip install Scrapy

## Create project
	scrapy startproject olx
	cd olx/
	scrapy genspider electronics  www.olx.in


## Test scrapy
	scrapy crawl   electronics
	scrapy crawl --nolog  electronics  #You can disable the debugger if you don’t want debugging information.

## Scrapy Shell
### Since entire DOM is available, you can play with it.
	scrapy shell https://www.olx.in/item/ps3-250gb-with-8-original-games-disc-1-controller-ID1qXSyF.html#506dd58b3b

## Save data in csv or json format
	scrapy crawl  electronics -o data.csv -t csv

you can even get data in JSON format, all you have to do is to pass json with -t switch.


### ToDoS
- [x] Simple web crawler
- [ ] Add single proxy
- [ ] Add multiple proxies
- [ ] Deal with captcha