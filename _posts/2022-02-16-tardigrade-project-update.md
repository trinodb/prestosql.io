---
layout: post
title:  "Tardigrade Project Update"
author: Andrii Rosa
excerpt_separator: <!--more-->
---

Over the last couple of months we’ve added support for full query retries, landed experimental support 
for task level retries and provided a proof of concept implementation of a distributed exchange plugin 
(description below). We are still working on improving scheduling algorithms as well as optimizing 
exchange plugin implementation to make the task level retries fully usable.

<!--more-->

Here is a quick summary of our progress so far:

* Added support for [automatic query retries](https://github.com/trinodb/trino/pull/9361). This functionality 
  is ready to use and can be enabled by setting the `retry_policy=QUERY` session property. Now 
  [it is possible](https://github.com/trinodb/trino/pull/10507) to enable automatic retries for queries that 
  produce more than `32MB` of output. Dynamic filtering is now also 
  [fully supported](https://github.com/trinodb/trino/pull/10274) with automatic query retries enabled.
* Landed an [initial set of changes](https://github.com/trinodb/trino/pull/9818) to support task level retries. 
  To be enabled, a plugin implementing the 
  [ExchangeManager](https://github.com/trinodb/trino/blob/master/core/trino-spi/src/main/java/io/trino/spi/exchange/ExchangeManager.java) 
  interface has to be installed.
* Landed a [proof of concept implementation](https://github.com/trinodb/trino/pull/10823) of the 
  [ExchangeManager](https://github.com/trinodb/trino/blob/master/core/trino-spi/src/main/java/io/trino/spi/exchange/ExchangeManager.java) 
  interface. The implementation is fully functional, however we are still [working on optimizing the read path](https://github.com/trinodb/trino/issues/11050). 
  Also for now, only S3 compatible file systems are supported.
* Added support for automatic retries in [Hive](https://github.com/trinodb/trino/issues/10252) and [Iceberg](https://github.com/trinodb/trino/pull/10622). 
  Supporting automatic retries for [JDBC based connectors](https://github.com/trinodb/trino/issues/10254) is up for grabs.
* Implemented [weight based split assignment](https://github.com/trinodb/trino/pull/10837) for balanced work distribution between fault tolerant tasks.
* Working on [adaptive sizing strategy for intermediate tasks](https://github.com/trinodb/trino/pull/11023) to minimize scheduling overhead 
  while keeping the cost of a single task failure at minimum. 
* Making progress on introducing an [advanced memory aware scheduling](https://github.com/trinodb/trino/pull/10432) that would allow us 
  to better support memory intensive queries, improve resource utilization and ensure fair resource allocation between queries.
* Started working on [supporting dynamic filtering](https://github.com/trinodb/trino/issues/9935) for queries with task level retries enabled.
* Working on [accommodating failed attempts](https://github.com/trinodb/trino/issues/10734) in various internal statistics reported by 
  the engine (e.g.: `QueryInfo`, `QueryCompletedEvent`). [UI changes](https://github.com/trinodb/trino/issues/10754) will come next.

Over the next couple of weeks we are planning to focus on:

* [Optimizing read path for the reference implementation of the exchange plugin](https://github.com/trinodb/trino/issues/11050)
* Landing [memory aware scheduling for fault tolerant execution](https://github.com/trinodb/trino/pull/10432)
* Landing [adaptive sizing for intermediate tasks](https://github.com/trinodb/trino/pull/11023)
* [Accommodating failed attempts into query statistics reporting](https://github.com/trinodb/trino/issues/10734)
* Making progress on [supporting dynamic filtering](https://github.com/trinodb/trino/issues/9935) for queries with task level retries enabled

The current state of development can be tracked by following this [issue](https://github.com/trinodb/trino/issues/9101).

Stay tuned!