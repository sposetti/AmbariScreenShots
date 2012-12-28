List Services
=====

[Back to Resources](index.md#resources)

Returns a collection of the services in a given cluster.

    GET /clusters/:name/services

**Response**

    200 OK
    {
    "href" : "http://your.ambari.server/api/v1/clusters/MyCluster/services",
    "items" : [
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
        }
      ]
    }
