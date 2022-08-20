---
title: "Quiplash Clone"
draft: true
---

This project was inspired by the game Quiplash made by Jackbox Games.
It has a Java Spring backend to store all of the game data on the server.
The frontend consists of Angular/Vue to act as frontend where the data is either displayed or gathered from the user.
Currently the frontend makes polling calls to the backend for updates on things such as the game phase when waiting on another player to complete a task.
A way to optimize this would be to use either websockets to keep open for the duration of the game or to utilize server push which is new in HTTP 2.
This project was built to handle multiple concurrent games with the option to use your own LAN server if necessary.

https://github.com/yodigi7/quiplash

# Tech Stack

* Java
* Spring
* Angular
* Vue
* h2
