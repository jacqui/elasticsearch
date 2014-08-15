## ElasticSearch Dockerfile


This is a fork of [Docker](https://www.docker.io/)'s [trusted build](https://index.docker.io/u/dockerfile/elasticsearch/) of [ElasticSearch](http://www.elasticsearch.org/).

It adds the following to the elasticsearch.yml config:

```
index:
  mapping:
    ignore_malformed: true
    analyzer:
      default:
        type: keyword
```

