Notification API
================

Most services on the web nowadays do not offer an unified way of notifications.
Which means that interoperability between these services is practically
non-existent or needs some sort of 'blessing' by the services.

One possible solution to such a problem would be a small and easily configurable
service that anyone can easily install on their webserver and then use to
orchestrate anything they would like.

This means that this notification service can be seen as a collection of
multiple source and single producer queues. A simple example:

```
                          +--------------+
    github.com ---------->| Notification |
                          |     API      |
                          |  Rule /mail  +------> Call http://example.com/cb
    gitlab.com ---------->|   On Commit  |
                          +--------------+
```

