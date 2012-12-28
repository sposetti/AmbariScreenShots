View Service Components
=====

[Back to Index](index.md)

Refers to a collection of all components for a given service.

    GET /clusters/:name/services/:serviceName/components

**Response**

    200 OK
    {
    "href" : "http://ec2-50-17-38-137.compute-1.amazonaws.com:8080/api/v1/clusters/MyIE9/services/HDFS/components",
    "items" : [
      {
      "href" : "http://ec2-50-17-38-137.compute-1.amazonaws.com:8080/api/v1/clusters/MyIE9/services/HDFS/components/DATANODE",
      "ServiceComponentInfo" : {
        "cluster_name" : "MyIE9",
        "component_name" : "DATANODE",
        "service_name" : "HDFS"
        }
      },
      {
      "href" : "http://ec2-50-17-38-137.compute-1.amazonaws.com:8080/api/v1/clusters/MyIE9/services/HDFS/components/SECONDARY_NAMENODE",
      "ServiceComponentInfo" : {
        "cluster_name" : "MyIE9",
        "component_name" : "SECONDARY_NAMENODE",
        "service_name" : "HDFS"
        }
      },
      {
      "href" : "http://ec2-50-17-38-137.compute-1.amazonaws.com:8080/api/v1/clusters/MyIE9/services/HDFS/components/NAMENODE",
      "ServiceComponentInfo" : {
        "cluster_name" : "MyIE9",
        "component_name" : "NAMENODE",
        "service_name" : "HDFS"
        }
      },
      {
      "href" : "http://ec2-50-17-38-137.compute-1.amazonaws.com:8080/api/v1/clusters/MyIE9/services/HDFS/components/HDFS_CLIENT",
      "ServiceComponentInfo" : {
        "cluster_name" : "MyIE9",
        "component_name" : "HDFS_CLIENT",
        "service_name" : "HDFS"
        }
      } ]
    }
