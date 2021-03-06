# [WIP] Grafana Flamegraph Panel

## Building flame graphs

[![Flame Graph Example](https://media.giphy.com/media/l41JMjBaxrZw1bqpi/giphy.gif)](http://spiermar.github.io/d3-flame-graph/)

Please read [Brendan Gregg's post](http://www.brendangregg.com/flamegraphs.html)

## Demo

**[Grafana live demo](https://grafana.flamgraph.samuel-berthe.fr/dashboard/db/demo-flamegraph?orgId=1)**

To generate metrics on the "demo" service, execute many times:

```
$ curl https://demo.flamgraph.samuel-berthe.fr
```

You will see some `pow()` calls in the graph.

Metrics are collected every 30 secondes, plz keep waiting if `pow()` is not shown on the flame graph.

## Live profiling

### Prometheus + NodeJS

[Prometheus exporter: Promfiler](github.com/samber/node-promfiler)

```
$ npm install -g promfiler
$ promfiler app.js
```

## Credits

This Grafana panel is based on the great library [d3-flamegraph](https://github.com/spiermar/d3-flame-graph), wrote by Spiermar. :clap: :clap:
