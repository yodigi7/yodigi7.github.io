---
title: "Websockets"
date: "2023-09-30"
description: "Websockets provide a bi-directional, full-duplex connection for real-time communication between clients and servers, ideal for applications like multiplayer games."
tags:
  - backend
---

## Introduction to Websockets
Websockets are a very cool technology that is a bi-directional full duplex protocol.
Bi-directional meaning that once the connection is open, either the server or the client can initiate transferring data.
This is different from typical webservers where the client is the one always initiating the request for information such as an HTTP web page.
Full duplex meaning that with one connection, the client can be sending information to the server while at the same time be receiving data from the server.

## My use case
I first came across this when working on my project for a [Quiplash clone]({{< ref "/projects/quiplash-clone" >}}).
For the project, there were multiple clients connecting to a server.
At the beginning of a round, each client would need to submit answers to questions at their own rate.
If a client finished early, they would need to constantly ping the server to ask if the round was over yet.
I implemented the solution to just have the client poll the server every second.
This is obviously a very inefficient solution that would not scale at all whatsoever.

Looking back on it now, using websockets would be perfect for this as the connection would be long lasting, it would last the entire duration of the game which would be around 15 minutes on average.
A long lasting connection is one factor that should be taken into account for websockets as they are more expensive to initiate but each subsequent transfer of information is cheaper than the average HTTP connection.
It would also be faster as it would have the least amount of latency because the server can decide when the round is over and can send an update to all of the clients.

## My Hide and Seek Game

I've been working on a hide and seek game where players are split into seekers and hiders. The game uses Websockets to allow real-time communication between clients and the server, ensuring smooth gameplay. As the hiders try to evade capture, the seekers are notified immediately when they get closer, creating a dynamic and engaging experience. The game is designed to be lightweight yet interactive, providing a fun and seamless multiplayer experience.

Check it out here: [Hide and Seek]({{< ref "/projects/hide-and-seek" >}}).

## Some useful resources
* Amazing YouTube channel from a backend/network engineer guru: https://www.youtube.com/watch?v=2Nt-ZrNP22A&ab_channel=HusseinNasser