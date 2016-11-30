# Example Voting App

This example is an adaptation of the Docker 3th birthday voting demo
app originally found in this repo:

	https://github.com/docker/docker-birthday-3

It's adapter to run on Kubernetes 1.2 and up.

##Architecture

* A Python webapp which lets you vote between two options
* A Redis queue which collects new votes
* A Java worker which consumes votes and stores them in…
* A Postgres database backed by a Docker volume
* A Node.js webapp which shows the results of the voting in real time
