Introduction
------------

The Collaborative Informatics and Neuroimaging Suite Toolkit for
Anonymous Computation, User Interface (COINSTAC) is software created to
foster collaborative research by removing large barriers to traditional
data-centric collaboration approaches. It is a desktop application that
can be run on the major three operating systems (Windows, Mac, and
Linux).

Installation
------------

Below are instructions for how to set up COINSTAC on your computer.
These instructions work for Ubuntu 16.04 and may work for later versions
of Ubuntu and other Debian-based systems (no guarantees). You may also
be able to run on CentOS, but we have not tested on any versions of that
OS.

The following steps should be taken, explained in more detail below:

1.  Verify System Requirements

2.  Install Docker

3.  Download and Run COINSTAC Application

Verify System Requirements
--------------------------

Use an Ubuntu 16.04 computer that has at least 8 GB of memory.

[https://docs.docker.com/install/linux/docker-ce/ubuntu/\#prerequisites](https://docs.docker.com/install/linux/docker-ce/ubuntu/#prerequisites)

Install Docker
--------------

Install Docker using the instructions in the link below.

[https://docs.docker.com/install/linux/docker-ce/ubuntu/](https://docs.docker.com/install/linux/docker-ce/ubuntu/)

### Verify Installation

Check that docker is installed by opening a terminal and typing:

> docker -v

You should see a similar message, probably with a different version and
build:

> Docker version 18.03.1-ce, build 9ee9f40

### Verify Docker is Running

Before starting COINSTAC, verify that Docker is running on your computer
by opening a terminal and typing:

> sudo systemctl status docker

### Running Docker

To run Docker, type the following into a terminal window:

> sudo systemctl start docker

Download and Run COINSTAC Application
-------------------------------------

### Download

To download the COINSTAC application, go to this page and download the
latest release:

[https://github.com/MRN-Code/coinstac/releases](https://github.com/MRN-Code/coinstac/releases)

-   Download the file named **coinstac-linux-x64.zip**.

-   After the download is complete, extract the zip file to a folder on
    your computer.

### Configure Docker Usage

Follow the below instructions taken from [here](https://docs.docker.com/engine/install/linux-postinstall/#manage-docker-as-a-non-root-user) to run Docker as a non-root user. 

Create the `docker` group

> sudo groupadd docker

Add your user to the `docker` group

> sudo usermod -aG docker $USER

Run this command to activate changes. If it does not work, log out and log back in.

> newgrp docker

Verify that you can run `docker` commands without `sudo`

> docker run hello-world

### Run Application

> ./coinstac
