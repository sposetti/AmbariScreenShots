View Cluster Information
=====

[Back to Index](index.md)

Returns information for the specified cluster identified by ":name"

    GET /clusters/:name

**Response**

{
  "href" : "http://ec2-50-17-38-137.compute-1.amazonaws.com:8080/api/v1/clusters/MyIE9",
  "Clusters" : {
    "cluster_name" : "MyIE9",
    "cluster_id" : 1,
    "version" : "HDP-1.2.0"
  },
  "requests" : [ ],
  "services" : [
    {
      "href" : "http://ec2-50-17-38-137.compute-1.amazonaws.com:8080/api/v1/clusters/MyIE9/services/NAGIOS",
      "ServiceInfo" : {
        "cluster_name" : "MyIE9",
        "service_name" : "NAGIOS"
      }
    },
    {
      "href" : "http://ec2-50-17-38-137.compute-1.amazonaws.com:8080/api/v1/clusters/MyIE9/services/HCATALOG",
      "ServiceInfo" : {
        "cluster_name" : "MyIE9",
        "service_name" : "HCATALOG"
      }
    },
    {
      "href" : "http://ec2-50-17-38-137.compute-1.amazonaws.com:8080/api/v1/clusters/MyIE9/services/PIG",
      "ServiceInfo" : {
        "cluster_name" : "MyIE9",
        "service_name" : "PIG"
      }
    },
    {
      "href" : "http://ec2-50-17-38-137.compute-1.amazonaws.com:8080/api/v1/clusters/MyIE9/services/WEBHCAT",
      "ServiceInfo" : {
        "cluster_name" : "MyIE9",
        "service_name" : "WEBHCAT"
      }
    },
    {
      "href" : "http://ec2-50-17-38-137.compute-1.amazonaws.com:8080/api/v1/clusters/MyIE9/services/MAPREDUCE",
      "ServiceInfo" : {
        "cluster_name" : "MyIE9",
        "service_name" : "MAPREDUCE"
      }
    },
    {
      "href" : "http://ec2-50-17-38-137.compute-1.amazonaws.com:8080/api/v1/clusters/MyIE9/services/GANGLIA",
      "ServiceInfo" : {
        "cluster_name" : "MyIE9",
        "service_name" : "GANGLIA"
      }
    },
    {
      "href" : "http://ec2-50-17-38-137.compute-1.amazonaws.com:8080/api/v1/clusters/MyIE9/services/HIVE",
      "ServiceInfo" : {
        "cluster_name" : "MyIE9",
        "service_name" : "HIVE"
      }
    },
    {
      "href" : "http://ec2-50-17-38-137.compute-1.amazonaws.com:8080/api/v1/clusters/MyIE9/services/HDFS",
      "ServiceInfo" : {
        "cluster_name" : "MyIE9",
        "service_name" : "HDFS"
      }
    },
    {
      "href" : "http://ec2-50-17-38-137.compute-1.amazonaws.com:8080/api/v1/clusters/MyIE9/services/ZOOKEEPER",
      "ServiceInfo" : {
        "cluster_name" : "MyIE9",
        "service_name" : "ZOOKEEPER"
      }
    },
    {
      "href" : "http://ec2-50-17-38-137.compute-1.amazonaws.com:8080/api/v1/clusters/MyIE9/services/SQOOP",
      "ServiceInfo" : {
        "cluster_name" : "MyIE9",
        "service_name" : "SQOOP"
      }
    },
    {
      "href" : "http://ec2-50-17-38-137.compute-1.amazonaws.com:8080/api/v1/clusters/MyIE9/services/HBASE",
      "ServiceInfo" : {
        "cluster_name" : "MyIE9",
        "service_name" : "HBASE"
      }
    },
    {
      "href" : "http://ec2-50-17-38-137.compute-1.amazonaws.com:8080/api/v1/clusters/MyIE9/services/OOZIE",
      "ServiceInfo" : {
        "cluster_name" : "MyIE9",
        "service_name" : "OOZIE"
      }
    }
  ],
  "hosts" : [
    {
      "href" : "http://ec2-50-17-38-137.compute-1.amazonaws.com:8080/api/v1/clusters/MyIE9/hosts/ip-10-36-113-130.ec2.internal",
      "Hosts" : {
        "cluster_name" : "MyIE9",
        "host_name" : "ip-10-36-113-130.ec2.internal"
      }
    },
    {
      "href" : "http://ec2-50-17-38-137.compute-1.amazonaws.com:8080/api/v1/clusters/MyIE9/hosts/ip-10-114-98-119.ec2.internal",
      "Hosts" : {
        "cluster_name" : "MyIE9",
        "host_name" : "ip-10-114-98-119.ec2.internal"
      }
    }
  ]
}

