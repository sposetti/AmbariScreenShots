View Component Information
=====

[Back to Index](index.md)

Refers to a specific component identified by ":componentName" for a given service.

    GET /clusters/:name/services/:serviceName/components/:componentName

**Response**

    200 OK
    {
    "href" : "http://your.ambari.server/api/v1/clusters/MyCluster/services/HDFS/components/DATANODE",
    "metrics" : {
      "rpc" : {
        ...
      },
      "dfs" : {
        "datanode" : {
          ...
        }
      },
      "disk" : {
        ...
      },
      "cpu" : {
        ...
      },
      "jvm" : {
        ...
      },
      "load" : {
        ...
      },
      "memory" : {
        ...
      },
      "network" : {
        ...
      },
    },
    "ServiceComponentInfo" : {
      "cluster_name" : "MyCluster",
      "component_name" : "DATANODE",
      "service_name" : "HDFS"
    },
    "host_components" : [
      {
      "href" : "http://your.ambari.server/api/v1/clusters/MyCluster/hosts/some.cluster.host/host_components/DATANODE",
      "HostRoles" : {
        "cluster_name" : "MyCluster",
        "component_name" : "DATANODE",
        "host_name" : "some.cluster.host"
        }
      } ]
    }
