View Service Components
=====

[Back to Resources](index.md#resources)

Refers to a collection of all components for a given service.

    GET /clusters/:name/services/:serviceName/components

**Response**

    200 OK
    {
    "href" : "http://your.ambari.server/api/v1/clusters/MyCluster/services/HDFS/components",
    "items" : [
      {
      "href" : "http://your.ambari.server/api/v1/clusters/MyCluster/services/HDFS/components/DATANODE",
      "ServiceComponentInfo" : {
        "cluster_name" : "MyCluster",
        "component_name" : "DATANODE",
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
      },
      {
      "href" : "http://your.ambari.server/api/v1/clusters/MyCluster/services/HDFS/components/NAMENODE",
      "ServiceComponentInfo" : {
        "cluster_name" : "MyCluster",
        "component_name" : "NAMENODE",
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
      } ]
    }
