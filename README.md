[![Build Status](https://travis-ci.org/chamaconekt/members.svg?branch=master)](https://travis-ci.org/chamaconekt/members) [![Coverage Status](https://coveralls.io/repos/github/chamaconekt/members/badge.svg?branch=master)](https://coveralls.io/github/chamaconekt/members?branch=master) [![Known Vulnerabilities](https://snyk.io/test/github/chamaconekt/members/badge.svg)](https://snyk.io/test/github/chamaconekt/members) [![bitHound Overall Score](https://www.bithound.io/github/chamaconekt/members/badges/score.svg)](https://www.bithound.io/github/chamaconekt/members) [![bitHound Dependencies](https://www.bithound.io/github/chamaconekt/members/badges/dependencies.svg)](https://www.bithound.io/github/chamaconekt/members/master/dependencies/npm) [![bitHound Dev Dependencies](https://www.bithound.io/github/chamaconekt/members/badges/devDependencies.svg)](https://www.bithound.io/github/chamaconekt/members/master/dependencies/npm) [![bitHound Code](https://www.bithound.io/github/chamaconekt/members/badges/code.svg)](https://www.bithound.io/github/chamaconekt/members) [![CLA assistant](https://cla-assistant.io/readme/badge/chamaconekt/members)](https://cla-assistant.io/chamaconekt/members) [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

# Chamaconekt-members Microservice 
This project manages the members business domain in the Chamaconekt Open Source platform.It is completely independent 
from other microservices.It has its own database that is utilised by other microservices via REST API.

# Getting started 
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. 
See deployment for notes on how to deploy the project on a live system.

## Prerequisites
- **Docker**
  - Installation instructions are available at the [Docker](https://www.docker.com/) website 
- **NodeJs**
  - Installation instructions are available at the [NodeJs](https://nodejs.org/) website 


# Installing

### Installing via Docker Images 
This instruction provides a simple way to incorporate chamaconekt-members into your private infrastructure through 
Docker Images.This image provides a default, non-validating, ephemeral configuration that should work for most developers.
This image is created via this [Dockerfile](https://github.com/chamaconekt/members/blob/master/Dockerfile)

```     $ docker pull chamaconektkenya/members       ```

### Running locally via Docker 
- **Build and run using Docker Compose:**
  - ```     $ git clone https://github.com/chamaconekt/members          ```
  - ```     $ cd members           ```
  - ```     $ docker-compose-up       ```


### Running Locally from GitHub

Clone this project from github 

```     $ git clone git@github.com:chamaconekt/members.git       ```

Change directory into the cloned repository 

```     $ cd members     ```

Install all of the project dependencies

```     $ npm install       ```

Start the development server

```     $ npm start         ```

The app is running at ``` http://localhost:3000/ ``` . Note that the development build is not optimized. To create a 
production build, use ```  $ npm run build     ```


# Running the tests

## Continuous Intergration Tests 
This project is running continuous intergration tests via [Travis CI](https://travis-ci.org) .This helps us intergrate code as oftern 
as possible and every commit is tested before and after being merged into the master branch by an automated build.This helps up our 
development process and minimizes the risk of critical issues in production.


## Vulnerability tests
This project is running vulnerability tests via [Snyk](https://snyk.io) and [Bithound](https://www.bithound.io) .Usually , open source is 
wesome for boosting our productivity. However, taking code written by others, often with little to no vetting of its security pedigree, 
can put our application at risk - a risk multiplied by the many dependencies a modern application uses. 


# Deployment

## Deploying to Docker Cloud
Docker Cloud makes it easy for new docker users to build and deploy their applications. Docker Cloud's operations
interface empowers seasoned Docker users to manage a full spectrum of applications, from single container apps to
distributed microservice stacks,anywhere.

### Prerequisites
-  docker-cloud CLI

__Installing  docker-cloud CLI ( Linux or Windows)__

```     $ pip install docker-cloud       ```

If you encounter errors on Linux machines, make sure that ``` $ python-dev ``` is installed. For example, on Ubuntu, run the 
following command: ``` $ sudo apt-get install python-dev ```

__Validate the installation__
Check that the CLI installed correctly:

``` $ docker-cloud -v   ```

__Docker cloud quickstart__

First, you should log in using the ``` docker ``` CLI and the ``` docker login ``` command. Your Docker ID, which you also use to log 
in to [Docker Hub](https://hub.docker.com/) , is also used for logging in to [Docker Cloud](https://cloud.docker.com/) .

Docker Cloud pulls up a stack fom the [docker-cloud.yml](https://github.com/chamaconekt/members/blob/master/docker-cloud.yml) 
file defined in this root repository. This is a logical grouping of the chamaconekt-members microservice that is 
deployed

[![Deploy to Docker Cloud](https://files.cloud.docker.com/images/deploy-to-dockercloud.svg)](https://cloud.docker.com/stack/deploy/)

This stack file will quickly deploy this cluster of microservice to a set of nodes.

# Contributing 

## How to contribute
We're striving to keep master's history with minimal merge bubbles. To achieve this, we're asking pull requests to be submitted 
on top of master.

## Finding things to work on
The first place to start is always looking over the current github issues for the project you are interested in contributing to.Issues 
marked with __help wanted__ are usually pretty self contained and a good place to get started. Chamaconekt also uses these same github 
issues to keep track of what we are working on.If you see any issues that are assigned to a particular person that means someone is 
currently working on that issue.Of course feel free to make your own issues if you think something needs to be added or fixed.


## Basic quality checks
Please ensure that all tests pass before submitting changes.Try to separate logically distinct changes into separate commits and 
thematically distinct commits into separate pull requests.

## Submitting changes
Please sign the [Contributor License Agreement](http://bit.ly/2gtLB0J). All content, comments, and pull requests must follow the
[Chamaconekt Community Guidelines](https://github.com/chamaconekt/members/blob/master/GUIDELINES.md)

Submit a pull request on top of master
- Include a descriptive commit message
- Changes contributed via pull requests should focus on a sigle issues at a time.

At this point you're waiting on us.We like to at least comment on pull requests within one week (and typically, three business days).
We may suggest some changes or improvements or alternatives.

# Versioning
We use [SemVer](http://semver.org/) for versioning.

# Authors
- [William Ondenge](https://github.com/wondenge)

# License
This project is licensed under the [Apache 2.0 License](https://www.apache.org/licenses/) 
- see the [LICENSE](https://github.com/chamaconekt/members/blob/master/LICENSE) file for details

# Acknowledgments
