# Dotnetty

https://github.com/Azure/DotNetty

## 1. Introduction

**DotNetty** is an open-source, asynchronous event-driven network application framework written in C# for building high performance network services

It's inspired by **Netty**, a Java network application framework

DotNetty simplifies **network programming**, such as TCP and UDP socket servers, by abstracting the complex threading and concurrency involved. It is used extensively in cloud, edge, and IoT applications

## 2. Main Components of DotNetty

**Bootstrap and ServerBootstrap**: These classes are used to **set up clients and servers**, respectively. They help configure and initiate network communication

**Channels**: The core component where all I/O operations occur

A channel represents an open connection to an entity such as a hardware device, a file, a network socket, etc

There are different types of channels for different types of I/O operations and protocols

**ChannelHandlers**: These are essentially event handlers that are attached to channels

They react to events like connection, disconnection, data received, etc

Handlers can be chained together to process inbound and outbound data (e.g., ByteToMessageDecoder, MessageToByteEncoder)

**EventLoopGroups**: These are groups of EventLoops that handle all the events in the lifecycle of a connection, such as accept, read, write, and close events

They are responsible for managing the threading model

**Buffers**: DotNetty provides ByteBuf for efficient data representation and manipulation, avoiding the overhead of Java's ByteBuffer flip operations

It's a powerful tool for working with byte data
