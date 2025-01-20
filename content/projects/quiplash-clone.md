---
title: "Quiplash Clone"
description: "Inspired by Quiplash, this project uses a Java Spring backend and Angular/Vue frontend to manage multiplayer games with server-side data handling. Current polling mechanisms could be optimized with WebSockets or HTTP/2 server push for real-time updates."
---

This project was inspired by the game Quiplash made by Jackbox Games.
It has a Java Spring backend to store all of the game data on the server.
The frontend consists of Angular/Vue to act as frontend where the data is either displayed or gathered from the user.
Currently the frontend makes polling calls to the backend for updates on things such as the game phase when waiting on another player to complete a task.
A way to optimize this would be to use either websockets to keep open for the duration of the game or to utilize server push which is new in HTTP 2.
This project was built to handle multiple concurrent games with the option to use your own LAN server if necessary.

https://github.com/yodigi7/quiplash

Here is a quick write-up on websockets and how I would redesign the connection part of this project today: [{{< ref "/technologies/websockets" >}}]({{< ref "/technologies/websockets" >}}/#my-use-case)

# Tech Stack

* Java
* Spring
* Angular
* Vue
* h2
