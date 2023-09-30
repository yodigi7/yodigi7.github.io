---
title: "gRPC"
---

# What is gRPC?
gRPC stands for Remote Procedure Protocol.
gRPC is an open-source, high-performance framework developed by Google.
It is designed for building efficient and fast communication systems, particularly in microservices architectures.
gRPC leverages HTTP/2, a protocol known for its speed and efficiency, making it an ideal choice for modern distributed systems.

___

# Key Benefits of gRPC

###### 1. Efficiency

gRPC uses Protocol Buffers (protobufs) as its interface definition language (IDL), resulting in compact and efficient data serialization.
This minimizes both bandwidth usage and processing time, leading to faster communication.

###### 2. Language Agnostic

gRPC supports multiple programming languages, allowing developers to seamlessly integrate services written in different languages.
This flexibility promotes interoperability and simplifies the development of heterogeneous systems.

###### 3. Bidirectional Streaming

gRPC supports bidirectional streaming, enabling real-time communication between clients and servers.
This feature is valuable for applications that require continuous data exchange, such as chat applications and online gaming.

###### 4. Automatic Code Generation

gRPC generates client and server code from the protobuf service definition, reducing boilerplate code and minimizing the risk of errors.

###### 5. Strong Typing

Protobufs provide a strong typing system, ensuring data consistency and reducing the chances of runtime errors.

###### 6. Security

gRPC includes built-in support for authentication, encryption, and authorization, making it a secure choice for communication over public networks.

# Conclusion

gRPC is a very interesting framework.
Personally the main times I would use it are going to be between backend services as there is not much support for full gRPC with browser clients.
I also would probably only do it with a more stable communication between two services as it is a lot easier to change the schema of a JSON object than a proto file that woud need to be regenerated for both the client and server.
gRPC takes a bit of effort to setup and maintain however the benefit would be most seen between two services who are very chatty and have a relatively high amount of network traffic since converting the payload to a byte object makes it much more efficient and faster that would be most seen in services that send large/a lot of payloads.
In general, I will probably continue using normal JSON payloads for most projects but I will keep this option in my back pocket for larger projects where efficiency matters most.


# Useful sources

* Official gRPC Documentaton: https://grpc.io/docs/languages/
* Official Protocol Buffers Documentaton: https://protobuf.dev/
* gRPC - YouTube: https://www.youtube.com/watch?v=Yw4rkaTc0f8&ab_channel=HusseinNasser
* Protocol Buffers - YouTube: https://www.youtube.com/watch?v=46O73On0gyI&ab_channel=HusseinNasser