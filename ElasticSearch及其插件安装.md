## 环境介绍

软件版本：ElasticSearch7.0.0     Kibana7.0.0

系统环境：mac 环境

## 安装过程

[官网](https://www.elastic.co/cn/downloads/elasticsearch)下载 ElasticSearch7.0.0 版本，下载后解压即可

进入es安装目录

```shell
cd elasticsearch-7.0.0
```

启动 es

```shell
bin/elasticsearch
```

如果报错的话直接给整个目录增加读写权限

在页面中访问 [http://localhost:9200/](http://localhost:9200/) 得到如下内容则表示安装成功

```json
{
  "name" : "anqideMacBook-Pro.local",
  "cluster_name" : "elasticsearch",
  "cluster_uuid" : "OrEZj_5_T62Zol1IIbkfSg",
  "version" : {
    "number" : "7.0.0",
    "build_flavor" : "default",
    "build_type" : "tar",
    "build_hash" : "b7e28a7",
    "build_date" : "2019-04-05T22:55:32.697037Z",
    "build_snapshot" : false,
    "lucene_version" : "8.0.0",
    "minimum_wire_compatibility_version" : "6.7.0",
    "minimum_index_compatibility_version" : "6.0.0-beta1"
  },
  "tagline" : "You Know, for Search"
}
```

## 安装Kibana

Kibana 是一个开源分析和可视化平台，旨在可视化操作 Elasticsearch 。Kibana可以用来搜索，查看和与存储在 Elasticsearch 索引中的数据进行交互。可以轻松地进行高级数据分析，并可在各种图表，表格和地图中显示数据。

Kibana 可以轻松理解海量数据。其简单的基于浏览器的界面使您能够快速创建和共享动态仪表板，实时显示 Elasticsearch 查询的更改。

**安装过程**

首先我们解压，然后进入目录

```shell
cd kibana-7.0.0-darwin-x86_64/
```

启动 kibana

```
bin/kibana
```

最后访问 [http://localhost:5601](http://localhost:5601) 即可进入管理界面，可以模拟数据，增加或者删除索引



