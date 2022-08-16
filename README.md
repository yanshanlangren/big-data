# big-data

# 此项目为大数据demo项目, 主要包含配置文件

# 环境配置

## 节点数量

3

## 机器配置

- CPU:2核
- RAM:4G 
- DISK:50G

## host配置

### /etc/hostname
分别替换为 node1,node2, node3

### /etc/hosts
192.168.0.26 node1 node1.hadoop.com
192.168.0.22 node2 node2.hadoop.com
192.168.0.21 node3 node3.hadoop.com

## 操作系统
CENTOS 7.9

## 软件环境
OPEN-JDK-8

### /etc/profile
```
export HADOOP_HOME=/home/hadoop/hadoop
export PATH=$PATH:$HADOOP_HOME/bin:$HADOOP_HOME/sbin


export HBASE_HOME=/home/hadoop/hbase
export PATH=$PATH:$HBASE_HOME/bin

export HIVE_HOME=/home/hadoop/hive
export HIVE_CONF_DIR=$HIVE_HOME/conf
export PATH=$HIVE_HOME/bin:$PATH

export SQOOP_HOME=/home/hadoop/sqoop
export PATH=$SQOOP_HOME/bin:$PATH


export HADOOP_CLASSPATH=$HADOOP_CLASSPATH:$HIVE_HOME/lib/*
```

