*Joseph Pierre-Louis & Tunwa Tongtawee - CS3700 - 11/10/2023*
# Project 5 - Web Crawler


## Approach

In order to implement this assignment, we started as simple as possible and continued to add features and complexity to the project in order to fulfill
all of the given requirements. We started with connecting, then sending simple HTTP messages. A large portion of our efforts on was spent on figuring out how to successfully login to the server before crawling. Then we just addded various optimizations, such as using a multithreading, a login retry system, and keep-alive to beef up our crawler and improve it until it was able to crawl through as necessary.
 

## Challenges

Our biggest challenge with this assignment was logging into the server because it was difficult to find the exact manner in which the server wanted our
POST message and also it was hard to figure out what the expected behavior of the server was.

## Testing

We tested the project using many print statements that allowed us to read HTTP response code and errors and various other useful information. We also used a print that output the number of links in queue and the links visited so we could keep track of the progress of the crawler.