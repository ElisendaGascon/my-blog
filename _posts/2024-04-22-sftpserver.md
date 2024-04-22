---
title: "Set up an SFTP server using Docker containers"
date: 2024-04-22
---
## How to get an SFTP server running locally using docker

SFTP is a network protocol that provides files access, file transfer, and file management over any reliable data stream. The protocol assumes that it is run over a secure channel, such as SSH, that the server has already authenticated the client, and that the identity of the client user is available to the protocol. 

In this post, I will go over how to get an SFTP server running locally using docker.

docker run -d -p 2036:22 sftp-server
sftp -oPort=2036 sftp_user@127.0.0.1
