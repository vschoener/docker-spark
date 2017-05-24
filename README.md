# docker-spark

This repo allows you to start a spark master node.

To keep it simple and as I'm experimenting this service, you need to do a couple things to get it running properly.

## Pre-require
None for now, Docker installed will help :)

## Install

First create the network (if you don't have it)
- docker network create ws_backend

Then build the image using our Makefile
- make build

## Run

Now we have our worker ready, you can simply run the following command
- make start

If you browse to the web ui of spark (IP:8080), you should see the server running

## Add worker ?
Yes it's possible to use this repo or use a docker command to start a worker. But you can also used my repo there https://github.com/vschoener/docker-spark-worker