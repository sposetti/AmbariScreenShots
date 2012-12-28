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




