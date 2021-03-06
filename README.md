# Scylla Operator
> Kubernetes Operator for Scylla (Pre-release version :warning:)

![](https://pbs.twimg.com/media/DwknrKJWkAE7qEQ.jpg)

## Quickstart

To quickly deploy a Scylla cluster on any Kubernetes cluster, follow the [quickstart guide](docs/quickstart.md).


## Description

The scylla-operator is a Kubernetes operator for managing scylla clusters. Currently it supports:
* Deploying multi-zone clusters
* Scaling up or adding new racks
* Scaling down
* Monitoring with Prometheus and Grafana

Future additions include:
* Integration with [Scylla Manager](https://docs.scylladb.com/operating-scylla/manager/)
* Version Upgrade
* Backups
* Restores


## Top-Performance Setup

Scylla performs the best when it has fast disks and direct access to the cpu. To deploy Scylla with maximum performance, follow the guide for your environment:
* [GKE](docs/gke/gke.md)


## Bugs

If you find a bug or need help running scylla, you can reach out in the following ways:
* `#kubernetes` channel on [Slack](https://scylladb-users-slackin.herokuapp.com/).
* File an [issue](https://github.com/scylladb/scylla-operator/issues) describing the problem and how to reproduce.

## Building the project

You can easily build Scylla Operator in your environment:
* Open the Makefile and change the `IMG` environment variable to a repository you have access to.
* Run `make publish` and wait for the image to be built and uploaded in your repo.

## Contributing

We would love for you to contribute to Scylla Operator, help make it even better and learn together! Use these resources to help you get started:
* `#scylla-operator` channel on [Slack](https://scylladb-users-slackin.herokuapp.com/).
* [Contributing Guide](docs/contributing.md)

## Acknowledgements

This project is based on cassandra operator, a community effort started by [yanniszark](https://github.com/yanniszark) of [Arrikto](https://www.arrikto.com/), as part of the [Rook project](https://rook.io/).


