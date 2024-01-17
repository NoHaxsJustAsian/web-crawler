* Tunwa Tongtawee & Joseph Pierre-Louis  - CS3700 - 11/10/2023*
# Project 5 - Web Crawler

## Introduction

This project, a part of the CS3700 course at Northeastern University, details our journey in developing a robust web crawler. The crawler is designed to interact with a server, handle login authentication, and efficiently navigate through web resources to gather specific data.

## Approach

Our strategy for implementing this assignment began with a straightforward approach, gradually introducing complexity and additional features. We started by establishing server connections and sending basic HTTP messages. A significant amount of effort was dedicated to figuring out the intricacies of logging into the server, a prerequisite for successful crawling. Subsequently, we introduced various optimizations including multithreading for concurrent operations, a login retry mechanism, and persistent connections (keep-alive) to enhance the efficiency and capability of our crawler.

## Challenges

The most daunting obstacle we encountered was the server login process. It proved challenging to discern the precise format required for POST messages, as well as understanding the server's expected responses and behavior. Overcoming this hurdle was critical to the success of our project.

## Testing

Our testing methodology relied heavily on the use of print statements. These were instrumental in allowing us to monitor HTTP responses, errors, and other pertinent information. We also implemented a logging mechanism to track the crawler's progress, specifically focusing on the number of links in the queue and the extent of links already visited.

## Features

- **Login Authentication:** Automated login using provided credentials.
- **Session Management:** Handles session cookies for continued access.
- **Link Discovery:** Parses HTML content to find and queue new links.
- **Data Extraction:** Searches for and stores specific data points (flags) from pages.
- **Error Handling:** Gracefully manages network errors and HTTP response codes.
- **Concurrency:** Uses threading to improve crawling efficiency.

## Usage

1. **Installation:** Clone the repository and install necessary Python dependencies.
2. **Configuration:** Set the target server, port, username, and password through command-line arguments.
3. **Execution:** Run the script to start the crawling process.

## Prerequisites

- Python 3
- Basic knowledge of network programming in Python
- Understanding of HTTP protocol and HTML structure

## Running the Crawler

To run the crawler, use the following command:

```bash
python3 crawler.py -s [server] -p [port] [username] [password]
