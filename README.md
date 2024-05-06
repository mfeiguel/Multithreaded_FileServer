# Multithreaded_FileServer

## Description
This is an implementation of a multithreaded file server that serves static files.
The client is multithreaded as well.

The client currently runs 7 threads with 14 file requests, this is why duplicates files will appear. Those duplicate requests are essentially to demonstrate the effective synchronization between the different threads.

## How to run
The server app was containerized using Docker and deployed in AWS ECS-Fargate. There is no need to run the server locally. The client will download the files from the deployed server when ran.

