List Clusters
=====

[Back to Index](index.md)

Returns a collection of the currently configured clusters.

    GET /clusters

**Response**

    200 OK
    {
      "href" : "http://your.ambari.server/api/v1/clusters",
      "items" : [ {
        "href" : "http://your.ambari.server/api/v1/clusters/MyCluster",
        "Clusters" : {
          "cluster_name" : "MyCluster",
          "version" : "HDP-1.2.0"
        }
      } ]
    }
