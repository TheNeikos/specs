API Overview
============

This specification describes a set of APIs for notification and management of
changes in distributed software projects. Each API targets a single problem. A
service might provide any set of these APIs, albeit the use of services not
supporting the core notification API is questionable.

A service providing any of the described APIs may bind them to different
interfaces. This way, a service provider may choose to expose the notification
API but expose some management API only locally, e.g. to improve security or
because the user is only handling private projects.

