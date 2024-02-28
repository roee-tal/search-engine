# Search Engine


This project is a compact implementation of a search engine employing a crawler to traverse specified websites. The crawler operates on a Breadth-First Search (BFS) algorithm, systematically navigating through links discovered within the crawled pages. Upon crawling each page, the system extracts its content, indexes it using Elasticsearch, and proceeds to explore additional links within the page.


## Technologies and Tools
### Database
- #### Redis:
   Used for storing visited links and other BFS crawler-related information (such as distance).
- #### ElasticSearch:
   Employed for indexing the content extracted from crawled pages.

### Message queue
- #### Kafka:
   Functions as the BFS queue.

### Containerization
- ### Docker:
   Utilized to run Kafka and Redis containers.

- This project is built around Java with the Spring Boot framework, utilizing Redis for efficient data storage related to the crawler's progress. Elasticsearch serves as the powerhouse for indexing crawled content, facilitating robust search capabilities.

- Additionally, the system offers flexibility with message brokers by supporting both Kafka , catering to diverse environments. The Docker containers ensure smooth deployment of Kafka and Redis, enabling seamless execution within varied setups.
