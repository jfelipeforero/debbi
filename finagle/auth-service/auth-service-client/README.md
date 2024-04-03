# auth-service-client

A Finagle Thrift client for auth-service.


### Creating a Client

    (auth-service.client/make-client "host:port")


You can call the methods defined by your Thrift service definition on this client.
The responses will all be wrapped in a Future (since this is an asynchronous operation).
The functions in `finagle-clojure.futures` can be used to transform the responses.