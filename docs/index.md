Ambari API Reference v1
=========

Release Version
----
Last Updated December 28, 2012

Getting Started
----

The Ambari API provides access to monitoring and metrics information of a Apache Hadoop cluster. This document is intended for developers who want to integrate with Ambari.

Authentication
----

The operations you perform against the Ambari API require authentication. Your access to the API requires the use of *Basic HTTP Authentication*. To use Basic Authentication, you need to send the *Authorization: Basic* header with your requests. For example, this can be handled when using curl and the --user option.

    curl --user name:password http://{your.ambari.server}/api/v1/clusters

_Note: The authentication method and source is configured at the Ambari Server. Changing and configuring the authentication method and source is not covered in this document._

Resources
----

Test
