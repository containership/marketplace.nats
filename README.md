# Nats

## What is the Containership Marketplace?

The Containership marketplace is a series of containerized applications configured to easily run and scale on a [containership.io](https://containership.io) cluster! Many conveniences such as High-Availability, automatic clustering among others are able to be configured out of the box allowing you to scale seamlessly as your infrastructure is required to grow.

> **Note:** If you attempt to run this image outside of a containership cluster, we cannot guarantee that it will run properly.

### Author
ContainerShip Developers - developers@containership.io

### Configuration
This image will run as-is, with no additional environment variables set. For clustering to work properly, start the application in host networking mode.

### Recommendations
* On your ContainerShip cluster, run this application using the `constraints.per_node=1` tag. Each node in your cluster will run an instance of gnatsd, creating a cluster of `n` hosts, where `n` is the number of follower hosts in your ContainerShip cluster.

## Contributing
Pull requests and issues are encouraged!
