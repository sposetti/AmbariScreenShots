View Service Information
=====

[Back to Resources](index.md#resources)

Refers to a specific service identified by ":serviceName" for a given cluster.

    GET /clusters/:name/services/:serviceName

**Response**

    200 OK
    {
    "href" : "http://your.ambari.server/api/v1/clusters/MyCluster/services/HDFS",
    "ServiceInfo" : {
      "cluster_name" : "MyCluster",
      "service_name" : "HDFS"
      },
    "components" : [
      {
      "href" : "http://your.ambari.server/api/v1/clusters/MyCluster/services/HDFS/components/NAMENODE",
      "ServiceComponentInfo" : {
        "cluster_name" : "MyCluster",
        "component_name" : "NAMENODE",
        "service_name" : "HDFS"
        }
      },
      {
      "href" : "http://your.ambari.server/api/v1/clusters/MyCluster/services/HDFS/components/DATANODE",
      "ServiceComponentInfo" : {
        "cluster_name" : "MyCluster",
        "component_name" : "DATANODE",
        "service_name" : "HDFS"
        }
      },
      {
      "href" : "http://your.ambari.server/api/v1/clusters/MyCluster/services/HDFS/components/HDFS_CLIENT",
      "ServiceComponentInfo" : {
        "cluster_name" : "MyCluster",
        "component_name" : "HDFS_CLIENT",
        "service_name" : "HDFS"
        }
      },
      {
      "href" : "http://your.ambari.server/api/v1/clusters/MyCluster/services/HDFS/components/SECONDARY_NAMENODE",
      "ServiceComponentInfo" : {
        "cluster_name" : "MyCluster",
        "component_name" : "SECONDARY_NAMENODE",
        "service_name" : "HDFS"
        }
      } ]
    }

