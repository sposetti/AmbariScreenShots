Ambari API Reference v1
=========

Release Version
----
_Last Updated December 28, 2012_

Getting Started
----

The Ambari API provides access to monitoring and metrics information of a Apache Hadoop cluster. This document describes the resources used in the Ambari API and is intended for developers who want to integrate with Ambari.

Authentication
----

The operations you perform against the Ambari API require authentication. Your access to the API requires the use of **Basic Authentication**. To use Basic Authentication, you need to send the **Authorization: Basic** header with your requests. For example, this can be handled when using curl and the --user option.

    curl --user name:password http://{your.ambari.server}/api/v1/clusters

_Note: The authentication method and source is configured at the Ambari Server. Changing and configuring the authentication method and source is not covered in this document._

Resources
----

There are 2 types of resources in the Ambari API:

- **Collection Resource:** This resource type refers to a collection of resources, rather than any specific resource. For example:

        /clusters  

  _Returns a collection of clusters_

- **Instance Resource:** This resource type refers to a single specific resource. For example:

        /clusters/MyCluster

  _Refers to the cluster resource identified by the id "MyCluster"_

### Clusters

- [List clusters](clusters.md)
- [View cluster information](clusters-cluster.md)

### Services

- [List services](services.md)
- [View service information](services-service.md)
- [View service components](components.md)
- [View component information](components-component.md)

### Hosts

- [List hosts](hosts.md)
- [View host information](hosts-host.md)
- [List host components](host-components.md)
- [View host component information](host-component.md)


Query Parameters
----

This mechanism limits which data is returned by a query based on a predicate(s). Providing query parameters does not result in any link expansion in the data that is returned to the client although it may result in expansion on the server to apply predicates on sub-objects.

_Note: Only applies to collection resources. And all URLs must be properly URL encoded_

**Query Operators**

<table>
  <tr>
    <th>Operator</th>
    <th>Example</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>=</td>
    <td>name=host1</th>
    <td>String or numerical equals</td>
  </tr>
  <tr>
    <td>!=</td>
    <td>host!=host1</th>
    <td>String or numerical not equals</td>
  </tr>
  <tr>
    <td>&lt;</td>
    <td>disk_total&lt;50</th>
    <td>Numerical less than</td>
  </tr>
  <tr>
    <td>&gt;</td>
    <td>disk_total&gt;50</th>
    <td>Numerical greater than</td>
  </tr>
  <tr>
    <td>&lt;=</td>
    <td>disk_total&lt;=50</th>
    <td>Numerical less than or equals</td>
  </tr>
  <tr>
    <td>&gt;=</td>
    <td>disk_total&gt;=50</th>
    <td>Numerical greater than or equals</td>
  </tr>
  <tr>
    <td>or</td>
    <td>disk_total&gt;50 or disk_free&lt;100</th>
    <td>Logial <code>or</code></td>
  </tr>
</table>

**Example: Get all hosts with less than 2 "cpu" or less than 100 "disk_total"**

    GET  /api/v1/clusters/c1/hosts?cpu/count<2 or metrics/disk/disk_total<100

    200 OK
    {
      “href” : “.../api/v1/clusters/MyCluster/hosts?property1=foo”,
      “items”: [
        {
            “href”: “.../api/v1/clusters/MyCluster/hosts/host1”
        },
        {
            “href”: ".../api/v1/clusters/MyCluster/hosts/host3”
        }
        ...
      ]
    }

Errors
----

This section describes how errors are represented in a response.

**Response**

    404 Not Found
    {
      “status”: 404,
      “message”: “standard message”,
      “developerMessage”: “verbose developers message”,
      “code”: 1234,
      “moreInfo”, “...”
    }

