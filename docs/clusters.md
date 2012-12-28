
List Clusters
=====

[Back to Index](index.md)

Returns a collection of the currently configured clusters.

    GET /clusters

Response

<code>
200 OK
{
    “href” : “http://ambari.server/api/v1/clusters”,
    “offset”: 0,
    “limit”: 10,
    “first”: “http://ambari.server/api/v1/clusters?offset=0”,
    “previous”: null,
    “next”: “http://ambari.server/api/v1/clusters?offset=10”,
    “last”: “http://ambari.server/api/v1/clusters?offset=?”,
    “items”: [
        {
            “href”: “http://ambari.server/api/v1/clusters/c1”
        },
        {
            “href”: “http://ambari.server/api/v1/clusters/c2”
        },
        {
            “href”: “http://ambari.server/api/v1/clusters/c3”
        }
        …
    ]
}
</code>
