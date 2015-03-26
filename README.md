# Sumatra Cloud

Sumatra Cloud is a Flask App for displaying and manipulating data
generated by the Sumatra simulation management tool. It has a web API
and a web front end. To run the API use

    $ python run.py --api

and to run the front end to view the data use

    $ python run.py --view

## [Sumatra]()

Sumatra is a command line tool that captures a lot of meta-data
pertaining to a Python execution. Sumatra is primarily aimed at
scientists using Python to run simulations, but the ideas could extend
to many other uses. The captured meta-data is not scientific specific,
but scientist often run the same script multiple times with only
slight modifications to parameter values. Version control alone is not
good at capturing this aspect of the scientific process.

## Why another Sumatra App?

The combination of Flask and MongoDB suits the Sumatra use case well
Flask is more readable and compact than Django and easier for a new
user to understand while MongoDB allows for more unstructured data
than an SQL database. Thus the amount of code required for the App is
reduced the App becomes more extensible to new tools and data
structures.


## [Doker][docker]
The cloud service has been 'dockerized'. If you want to build the
containers yourself. The Dockerfile at the root is configured for
the cloud service app and the one inside the docker/mongodb folder for
the database mongodb
With Docker we provide you two choices.

## Choice 1
You can pull this repository and build the docker containers yourself.
Refer to the [installation guide](INSTALLATION.md) on the docker
section 1 to figure out how to build and run those containers.

## Choice 2
The two containers are publicly shared on: 
[Docker registry][registery].
Refer to the [installation guide](INSTALLATION.md) on the docker
section 2 to figure out how to pull and run those containers.


## License

[The MIT license.][LICENSE]

## Instances

There are no current instances of the App, but we're working on making
an instance available.

## Prerequisites and Installation

See the [installation guide](INSTALLATION.md).

[docker]: https://www.docker.com/
[registery]: https://registry.hub.docker.com/repos/palingwende/