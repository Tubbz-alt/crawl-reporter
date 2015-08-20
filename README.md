# crawl-reporter

Indefinitely report latest crawl metrics from db to graphite

```
Usage: crawl-reporter [options] [command]

Commands:

  live <max> <timeout> Indefinitely process crawls taken from queue
  
```

## Arguments

#### Command line
* max     : the max amount of async reporters to have running at once
* timeout : how long to wait between checking for messages

#### Environment
* sqs queue URL : `SQS_URL`
* database URL  : `DATABASE_URL`
* graphite URL  : `GRAPHITE_URL` (not used)
