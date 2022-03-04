---
layout: default
menu_id: resources
title: Resources
show_hero: true
---

<div class="container__resources">
<div class="container">
<div class="row">

<div class="col-sm-12 col-md-4 col-lg-3 spacer-20 order-md-2 resourcesAnchors toc-styles">
<div markdown="1" class="rightcol toc-sticky">

### Resources

* [Client libraries](#libraries)
* [BI tools and notebooks](#ui)
* [Management tools](#tools)
* [Enterprise support](#support)
* [Managed services](#managed)
* [Cloud](#cloud)
  * [Amazon Web Services](#aws)
  * [Google Cloud](#gcp)
  * [Microsoft Azure](#azure)

</div></div>

<div class="col-sm-12 col-md-8 col-lg-9 spacer-20">

<div class="resourcesMain">
<div markdown="1" class="leftcol widecol faq">

## Client libraries {#libraries}

The following client libraries can be used to run queries from several
programming languages, and programs using the related platform:

* [Trino JDBC driver](docs/current/installation/jdbc.html) for Java/JVM
* [Starburst ODBC driver](https://www.starburst.io/platform/starburst-enterprise/) for Windows
* [trino-go-client]({{site.github_org_url}}/trino-go-client) for Go
* [presto-client-node](https://github.com/tagomoris/presto-client-node) for Node.js
* [lento](https://github.com/vweevers/lento) for Node.js
* [dbt adapter](https://github.com/starburstdata/dbt-trino)
* [trino-python-client]({{site.github_org_url}}/trino-python-client) for Python
* [PyHive](https://github.com/dropbox/PyHive) for Python
* [RPresto](https://github.com/prestodb/RPresto) for R
* [trino-client-ruby](https://github.com/treasure-data/trino-client-ruby) for Ruby

</div></div>

<div class="resourcesMain">
<div markdown="1" class="leftcol widecol faq">

## BI tools and notebooks {#ui}

<div markdown="1" class="item">

#### [Quix](https://wix.github.io/quix/)

Quix is a multi-user, easy-to-use notebook manager.
By utilizing Trino it provides unified access to
multiple data sources and effectively acts as a shared
space for your company's BI insights and know-how.

</div>

<div markdown="1" class="item">

#### [Redash](https://redash.io/)

Redash is a take on freeing the data within our company in a way
that will better fit our culture and usage patterns. It has Trino
support as well as other backends, and offers a query editor with
syntax highlighting and completion, and creating visualizations and
dashboards from query results.

</div>

<div markdown="1" class="item">

#### [Apache Superset](https://superset.apache.org/)

Apache Superset enables users to consume data in many different ways:
writing SQL queries, creating new tables, creating a visualization
(slice), adding that visualization to one or many dashboards and
downloading a CSV. SQL Lab is a a part of Superset and provides a rich
SQL editor that enables users to both query and visualize data. You
can explore and preview tables in Trino, effortlessly compose SQL
queries to access data. From there, you can either export a CSV file
or immediately visualize your data in the Superset "Explore" view.

</div>

<div markdown="1" class="item">

#### [yanagishima](https://yanagishima.github.io/yanagishima/)

yanagishima is a web application for Trino. yanagishima provides
the ability to execute query, show query, kill query, bookmark
query, search table, share query/query result, format query,
download as CSV/TSV file, insert chart, substitute query parameter,
and so on.

</div>

<div markdown="1" class="item">

#### [Hue](http://gethue.com/)

Hue is a mature open source SQL assistant for querying databases and data
warehouses. It is used by Fortune 500 companies, and focused on smart query
typing. Follow the [instructions to use the Trino
connector](https://docs.gethue.com/administrator/configuration/connectors/#trino)
to get started.

</div>

</div></div>

<div class="resourcesMain">
<div markdown="1" class="leftcol widecol faq">

## Management tools {#tools}

<div markdown="1" class="item">

#### [Presto-Gateway](https://github.com/lyft/presto-gateway)

Presto-Gateway is a gateway/proxy/load-balancer for multiple Trino clusters.
Users can register/de-register Trino clusters behind the gateway and connect to
it using standard clients.

</div>

<div markdown="1" class="item">

#### [Workload Analyzer](https://github.com/varadaio/presto-workload-analyzer)

The Workload Analyzer collects Trino workload statistics, and analyzes them.
The resulting [report](https://varada.io/wa-sample-report) provides improved visibility
into your analytical workloads, and enables cluster performance optimization.
For installation, see [here](https://github.com/varadaio/presto-workload-analyzer/blob/main/INSTALL.md).

</div>

</div></div>

<div class="resourcesMain">
<div markdown="1" class="leftcol widecol faq">

## Enterprise support {#support}

<div markdown="1" class="item">

#### [Starburst](https://www.starburst.io/)

Enterprise 24/7 support, installation, configuration, training,
custom development, tuning

At Starburst, our team is a major contributor to the open source
Trino project. We consist of many of the **experts and maintainers**
who have been contributing to and advancing the Trino product over
the last few years. Starburst provides [Starburst Enterprise, a fully supported,
enterprise ready Trino distribution](https://www.starburst.io/platform/starburst-enterprise/).
Starburst's distribution of Trino consists of additional tooling
and configurations to make it work well in the enterprise. Further,
it is rigorously tested at scale and patched as needed. With our
wide range of services, support, and training we help you be
successful in this new world of open source technologies in the
enterprise.

In addition to implementing Trino internals to make it the most
reliable, robust, and performant open source distributed query
engine, our team at Starburst is dedicated to continually improve
and add the needed features for the enterprise. Our major enterprise
focus areas are ease-of-use, security, robustness, wide range of
integrations, and reliable support SLAs.

</div>
<div markdown="1" class="item">

#### [Qubole](https://www.qubole.com/developers/presto-on-qubole/)

Enterprise 24/7 Support, HotFixes, Multiple Trino Versions, Backporting of critical
open source fixes and enhancements, Configuration, Tuning

Qubole has been offering a managed Trino service since 2014.
Qubole offers multiple Trino versions across multiple clouds
(AWS, Azure and Google Cloud) and maintains a regular upgrade process.
Qubole offers 24/7 support through its support and engineering
teams spread across the globe. Qubole hotfixes critical production
issues or major issues addressed in open source community. Qubole
also backports critical fixes and major enhancements from recent
versions of Trino to older versions. Qubole helps its users configure
their clusters, fine tune their workloads and get the best out of Trino.

</div>

</div></div>

<div class="resourcesMain">
<div markdown="1" class="leftcol widecol faq">

## Managed services {#managed}

<div markdown="1" class="item">

#### [Starburst Galaxy](https://www.starburst.io/platform/starburst-galaxy/)

Starburst Galaxy is the leading SaaS offering of Trino. It is capable of running
clusters in all major clouds, and is fully managed for you by Starburst.

It includes a rich user interface with query editor, query history, cluster
management, security configuration, and much more. Watch one
of the demo videos and find details in the [comprehensive user
documentation](https://docs.starburst.io/starburst-galaxy/index.html).

</div>

<div markdown="1" class="item">

#### [Trino on Qubole](https://www.qubole.com/developers/presto-on-qubole/)

Qubole has been offering a managed Trino service since 2014.
Qubole has optimized Trino for the cloud. Qubole’s enhancements
allow for dynamic cluster sizing, based on workload and termination
of idle clusters — ensuring high reliability while reducing compute
costs.

Qubole offers multiple Trino versions across multiple clouds
(AWS, Azure and Google Cloud) and maintains a regular upgrade process.
Qubole blends the latest features from the open source community
with Qubole’s proprietary solutions that boost performance,
lower cost, improve user experience, and provide smooth
administration of Trino clusters.

</div>

<div markdown="1" class="item">

#### [Amazon Athena](https://aws.amazon.com/athena/)

Amazon Athena is an interactive query service based on an older version of Trino
that makes it easy to analyze data in Amazon S3 using standard SQL.
Athena is serverless, so there is no infrastructure to manage, and
you pay only for the queries that you run.
Amazon Athena uses Trino with full standard SQL support and works
with a variety of standard data formats. Athena is out-of-the-box
integrated with AWS Glue Data Catalog, allowing you to create a
unified metadata repository across various services, crawl data
sources to discover schemas and populate your Catalog with new and
modified table and partition definitions, and maintain schema
versioning.

</div>

</div></div>

<div class="resourcesMain">
<div markdown="1" class="leftcol widecol faq">

## Cloud {#cloud}

Trino is readily available in [AWS](#aws) and [Azure](#azure)
cloud environments.

### AWS {#aws}

<div markdown="1" class="item">

#### [Starburst Enterprise on AWS](https://www.starburst.io/platform/deployment-options/aws/)

Starburst Enterprise on AWS combines the reliable, scalable, and
cost-effective cloud computing services provided by Amazon Web
Services (AWS) with the power of Trino, the fastest growing
distributed SQL query engine within the industry.

Through the use of Starburst’s CloudFormation template and Starburst
Trino AMI, Starburst Enterprise on AWS enables you to run analytic SQL
queries across a wide variety of data sources with elastic scaling
and usage-based pricing. Read more how to use Trino on AWS on our
[AWS Documentation site](https://docs.starburst.io/latest/aws.html).

</div>

<div markdown="1" class="item">

#### [Trino on Qubole on AWS](https://us.qubole.com/)

Qubole offers a managed Trino service on AWS that is optimized
for the cloud. Qubole supports cluster autoscaling based on
workload and termination of idle clusters — ensuring high
reliability while reducing compute costs. Qubole supports usage
of spot nodes on AWS with built in failure resilience around spot
termination notification handling and query retries. With Trino
on Qubole, users can create heterogenous clusters with spot nodes
from similar instance families that can further help reduce
compute costs.

</div>

<div markdown="1" class="item">

#### [Amazon EMR](https://aws.amazon.com/emr/)

Amazon EMR provides a managed Hadoop framework that makes it easy,
fast, and cost-effective to process vast amounts of data across
dynamically scalable Amazon EC2 instances. With EMR, you can launch
a large Trino cluster in minutes. You don't need to worry about
node provisioning, cluster setup or tuning.

Using Trino on EMR provides these benefits to customers:
* Elasticity: With Amazon EMR, you can provision one, hundreds, or
  thousands of compute instances to process data at any scale. You
  can easily increase or decrease the number of instances manually
  or with Auto Scaling, and you only pay for what you use.
* Simple and predictable pricing: You pay a per-second rate for
  every second used, with a one-minute minimum charge.

</div>

### Azure {#azure}

<div markdown="1" class="item">

#### [Starburst Enterprise on Azure](https://www.starburst.io/platform/deployment-options/starburst-on-azure/)

Starburst Enterprise is available via the Azure Marketplace.

</div>

<div markdown="1" class="item">

#### [Trino on Qubole on Azure](https://azure.qubole.com/)

Qubole offers a managed Trino service on Azure that is optimized
for the cloud. Qubole supports cluster autoscaling based on
workload and termination of idle clusters — ensuring high
reliability while reducing compute costs. Qubole supports
both Gen1 and Gen2 of Azure Data Lake Storage (ADLS) as well as
Azure Blob Storage.

</div>

### Google Cloud {#gcp}

<div markdown="1" class="item">

#### [Starburst Enterprise on Google Cloud](https://www.starburst.io/platform/deployment-options/starburst-on-google-cloud/)

Starburst Enterprise is available via the Google Cloud Marketplace.

#### [Trino on Qubole on Google Cloud](https://console.cloud.google.com/marketplace/details/qubole-public/qubole-data-service)

Qubole offers a managed Trino service on Google Cloud that is optimized
for cloud and is integrated with
[Google Cloud marketplace](https://console.cloud.google.com/marketplace/details/qubole-public/qubole-data-service).
Qubole supports cluster autoscaling based on workload and
termination of idle clusters — ensuring high reliability while
reducing compute costs. Qubole supports use of preemptible VMs in
its autoscaling to reduce costs. Qubole has also added support for
faster detection of query failures in Trino caused by preemptible
VM interruption.

</div>

</div></div>

</div></div></div>
