- [Prometheus常用命令行参数](#prometheus常用命令行参数)
  - [指定Prometheus配置文件](#指定prometheus配置文件)
  - [指定TSDB路径](#指定tsdb路径)
  - [指定数据存储时间](#指定数据存储时间)
  - [提供类似Nginx的reload功能](#提供类似nginx的reload功能)
  - [如果用k8s的deployment管理要开启](#如果用k8s的deployment管理要开启)

# Prometheus常用命令行参数

## 指定Prometheus配置文件

```shell
--config.file=/path/to/prometheus.yml
```

## 指定TSDB路径

```shell
--storage.tsdb.path=/path/to/prometheus_tsdb
```

## 指定数据存储时间

```shell
--storage.tsdb.retention.time=24h
```

## 提供类似Nginx的reload功能

```shell
--web.enable-lifecycle
```

## 如果用k8s的deployment管理要开启

```shell
--storage.tsdb.no-lockfile
```

