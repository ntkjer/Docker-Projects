# Link Extractor
A web application to extract links and anchor texts from a given web page and analyze link statistics.


* Another `Dockerfile` is added for the PHP web application to avoid live file mounting
* A Redis container is added for caching using the official Redis Docker image
* The API service talks to the Redis service to avoid downloading and parsing pages that were already scraped before

## Usage

```
$ docker-compose up --build
```

Open http://localhost/?url=http%3A%2F%2Fodu.edu%2F in a web browser.

Press `Ctrl + C` to terminate the service.
