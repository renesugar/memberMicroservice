

# Installation via Docker Images

This project provides a simple way to incorporate chamaconekt-members and other microservices into your private
infrastructure , provided that you use docker.

This image provides a default, non-validating, ephemeral configuration that should work for most developers.
By configuring a container using this image with a host-based volume (described below in the "Usage" section)
an operator gains access to full configuration , customization and persistance of data.

The image uses the following software:

# Usage

To use this project successfully, you should first decide a few things:

First, you must decide whether you will use a docker volume or not.When not using a volume, we say that the 
container is in _ephemeral mode_, that is nothing will be persisted between the runs of the container. 
Persistent mode is the alternative, which should be used in the case that you need to either customize your
configuration . We recommend persistent mode for anything besides a development or test environment.

Finally, you must decide what ports to expose.


