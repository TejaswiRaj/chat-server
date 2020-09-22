Chat Server

Simple chatroom in C loosely based on IRC. This project demonstrates the basic use of sockets. There is no client available but any telnet client will do. Just connect to the server on the specified port and address. By default port 1234 is used. This code runs on Linux.

## Build

Run makefile from repository

`make`

Then start

`./chat_server`


## Features

* Small code base (< 350 LOC)
* Accept multiple client (max 100)
* Name and rename usernames
* Send  messages
* Easily extenable

## Chat commands

| Command       | Parameter             |                                     |
| ------------- | --------------------- | ----------------------------------- |
| /quit         |                       | Leave the chatroom                  |
| /join         |                       | Server Join			      |
| /topic        | [message]             | Set the roomname chatroom topic     |
| /username     | [nickname]            | Change username                     |
| /msg          | [reference] [message] | Send message                        |
| /list         |                       | Show active clients                 |
| /help         |                       | Show this help                      |

There's no client file, telnet can be used to connect with server for multiple clients
Ex: telnet IP-address 1234
