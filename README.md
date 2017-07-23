# JAX-RS Sample application for Wildfly
A very simple JAX-RS sample application that implements a single JAX-RS service.  

Deployment
----

To build, simply run

```mvn clean package```

This will create a war file that can be deployed into an JEE app server.  I've only
tested with Wildfly at this point.

The war file can be deployed to Wildfly and possibly other JEE application servers.
For Wildlfy, there are many options to deploy listed on
[the application deployment page](https://docs.jboss.org/author/display/WFLY10/Application+deployment)
that can help deploy.

Sample Service Info
----
There is one service endpoints:

```GET /rest/v1/heartbeat``` - returns a "text/plain" HTTP body of "OK" if the service is up
  and running. A heartbeat service like this is commonly used in load balancing
  environments so that a load balancer can validate that an application is healthy.


Copyright (c) 2017
by Xigole Systems
Licensed under the Apache License - see the file LICENSE for details. 
