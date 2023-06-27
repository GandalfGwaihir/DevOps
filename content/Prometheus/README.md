![](https://images.contentstack.io/v3/assets/blt300387d93dabf50e/blt7326dcd379e54877/5913192559b80e7305b1045d/Screen-Shot-2016-09-02-at-10.08.13.png?format=webp&width=1200)

### [Prometheus](https://prometheus.io/) is an open-source systems monitoring and alerting toolkit originally built at SoundCloud. Since its inception in 2012, many companies and organizations have adopted Prometheus, and the project has a very active developer and user community. It is now a standalone open source project and maintained independently of any company.


# Features

Prometheus's main features are:

* a multi-dimensional data model with time series data identified by metric name and key/value pairs
* PromQL, a flexible query language to leverage this dimensionality
* no reliance on distributed storage; single server nodes are autonomous
* time series collection happens via a pull model over HTTP
* pushing time series is supported via an intermediary gateway
* targets are discovered via service discovery or static configuration
* multiple modes of graphing and dashboarding support

# Architecture

![](https://prometheus.io/assets/architecture.svg)

The Prometheus ecosystem consists of multiple components, many of which are optional:

* the main Prometheus server which scrapes and stores time series data
* client libraries for instrumenting application code
* a push gateway for supporting short-lived jobs
* special-purpose exporters for services like HAProxy, StatsD, Graphite, etc.
* an alertmanager to handle alerts
* various support tools

Most Prometheus components are written in Golang, making them easy to build and deploy as static binaries.