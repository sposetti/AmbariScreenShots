Ambari API Reference v1
=========

Release Version
----
Last Updated December 28, 2012

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

There are 2 types of resources in the Ambari Monitoring REST API.

- **Collection Resource:** This resource type doesn’t refer to any specific resource; rather it refers to a collection of resources. For example:

        /clusters  

  Returns a collection of clusters

- **Instance Resource:** This resource type refers to a single specific resource. For example:

        /clusters/cluster1

  Refers to the cluster resource identified by the id “cluster1”

<table>
  <tr>
    <th>Resources</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>
<code>/clusters</code>
    </td>
    <td>
Returns a collection of the currently configured clusters.
    </td>
  </tr>
  <tr>
    <td>
<code>/clusters/:name</code>
    </td>
    <td>
Returns information for a specific cluster.
    </td>
  </tr>
  <tr>
    <td>
<code>/clusters/:name/services</code>
    </td>
    <td>
Returns a collection of the services in a given cluster.
    </td>
  </tr>
  <tr>
    <td>
<code>/clusters/:name/services/:serviceName</code>
    </td>
    <td>
Returns information for a specific service in a given cluster.
    </td>
  </tr>
  <tr>
    <td>
<code>/clusters/:name/services/:serviceName/components</code>
    </td>
    <td>
Returns a collection of all components for the given service.
    </td>
  </tr>
  <tr>
    <td>
<code>/clusters/:name/services/:serviceName/components/:componentName</code>
    </td>
    <td>
Returns information for a specific component in a given service.
    </td>
  </tr>
  <tr>
    <td>
<code>/clusters/:name/hosts</code>
    </td>
    <td>
Returns a collection of all hosts in a given cluster.
    </td>
  </tr>
  <tr>
    <td>
<code>/clusters/:name/hosts/:hostName</code>
    </td>
    <td>
Returns information about a single host in a given cluster.

  <tr>
    <td>
<code>/clusters/:name/hosts/:hostName/host_components</code>
    </td>
    <td>
Returns a collection of components running on a given host.
    </td>
  </tr>
  <tr>
    <td>
<code>/clusters/:name/hosts/:hostName/host_components/:componentName</code>
    </td>
    <td>
Returns information for a specific role on the given host.
    </td>
  </tr>
</table>


