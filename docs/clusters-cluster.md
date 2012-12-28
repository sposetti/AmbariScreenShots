View Cluster Information
=====

[Back to Index](index.md)

Returns information for the specified cluster identified by ":name"

    GET /clusters/:name

**Response**

    200 OK
    {
      "href" : "http://your.ambari.server/api/v1/clusters/MyCluster",
      "Clusters" : {
        "cluster_name" : "MyCluster",
        "cluster_id" : 1,
        "version" : "HDP-1.2.0"
      },
      "services" : [
        {
        "href" : "http://your.ambari.server/api/v1/clusters/MyCluster/services/NAGIOS",
        "ServiceInfo" : {
          "cluster_name" : "MyCluster",
          "service_name" : "NAGIOS"
          }
        },
        {
        "href" : "http://your.ambari.server/api/v1/clusters/MyCluster/services/HCATALOG",
        "ServiceInfo" : {
          "cluster_name" : "MyCluster",
          "service_name" : "HCATALOG"
          }
        },
        {
        "href" : "http://your.ambari.server/api/v1/clusters/MyCluster/services/PIG",
        "ServiceInfo" : {
          "cluster_name" : "MyCluster",
          "service_name" : "PIG"
          }
        },
        {
        "href" : "http://your.ambari.server/api/v1/clusters/MyCluster/services/MAPREDUCE",
        "ServiceInfo" : {
          "cluster_name" : "MyCluster",
          "service_name" : "MAPREDUCE"
          }
        },
        {
        "href" : "http://your.ambari.server/api/v1/clusters/MyCluster/services/GANGLIA",
        "ServiceInfo" : {
          "cluster_name" : "MyCluster",
          "service_name" : "GANGLIA"
          }
        },
        {
        "href" : "http://your.ambari.server/api/v1/clusters/MyCluster/services/HIVE",
        "ServiceInfo" : {
          "cluster_name" : "MyCluster",
          "service_name" : "HIVE"
          }
        },
        {
        "href" : "http://your.ambari.server/api/v1/clusters/MyCluster/services/HDFS",
        "ServiceInfo" : {
          "cluster_name" : "MyIE9",
          "service_name" : "HDFS"
          }
        },
        {
        "href" : "http://your.ambari.server/api/v1/clusters/MyCluster/services/ZOOKEEPER",
        "ServiceInfo" : {
          "cluster_name" : "MyCluster",
          "service_name" : "ZOOKEEPER"
          }
        },
        {
        "href" : "http://your.ambari.server/api/v1/clusters/MyCluster/services/HBASE",
        "ServiceInfo" : {
          "cluster_name" : "MyCluster",
          "service_name" : "HBASE"
          }
        },
        {
        "href" : "http://your.ambari.server/api/v1/clusters/MyCluster/services/OOZIE",
        "ServiceInfo" : {
          "cluster_name" : "MyCluster",
          "service_name" : "OOZIE"
          }
        } ],
    "hosts" : [
      {
      "href" : "http://your.ambari.server/api/v1/clusters/MyCluster/hosts/some.cluster.host",
      "Hosts" : {
        "cluster_name" : "MyCluster",
        "host_name" : "some.cluster.host"
        }
      },
      {
      "href" : "http://your.ambari.server/api/v1/clusters/MyCluster/hosts/another.cluster.host",
      "Hosts" : {
        "cluster_name" : "MyCluster",
        "host_name" : "another.cluster.host"
        }
      } ]
    }

