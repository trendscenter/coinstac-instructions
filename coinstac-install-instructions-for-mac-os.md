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

To install and run COINSTAC, follow the below instructions:

1.  Verify System Requirements

2.  Install Docker

3.  Download and Run COINSTAC Application

Verify System Requirements
--------------------------

Use a Mac with OS X 10.12 or higher. Before starting, please check that
your computer meets the [System
Requirements](https://docs.docker.com/docker-for-mac/install/#what-to-know-before-you-install)
for Docker.

Install Docker
--------------

Install Docker from the link below.

[https://store.docker.com/editions/community/docker-ce-desktop-mac](https://store.docker.com/editions/community/docker-ce-desktop-mac)

### Verify Installation

Check that docker is installed by opening a terminal and typing:

> docker -v

You should see a similar message, probably with a different version and
build:

> Docker version 18.03.1-ce, build 9ee9f40

### Verify Docker is Running

Before starting COINSTAC, verify that Docker is running on your computer
by using one of the methods below.

#### Method \#1

You can verify that Docker is running by hovering over the Docker icon
<img src="https://github.com/trendscenter/coinstac-instructions/blob/markdown/install-mac/media/image1.png" width="20"
height="20"/> on your taskbar. You should see a message
that Docker is running.

#### Method \#2

Open a terminal and type:

> docker ps

You should see an output like this:

> CONTAINER ID IMAGE COMMAND CREATED STATUS PORTS NAMES

If you see an error message, then you have to start Docker.

### Running Docker

To run Docker:

-   Click on the Launchpad
    <img src="https://github.com/trendscenter/coinstac-instructions/blob/markdown/install-mac/media/image2.png" width="20" height="20"/> in your taskbar at the bottom of the screen.

-   Find Docker
    <img src="https://github.com/trendscenter/coinstac-instructions/blob/markdown/install-mac/media/image3.png" width="20" height="20"/> in your list of applications and click on it.

Download and Run COINSTAC Application
-------------------------------------

### Download

To download the COINSTAC application, do the following:

-   Go to this page and download the latest release:

    <https://github.com/MRN-Code/coinstac/releases/>

-   Download the file named **coinstac-darwin-x64.zip**.

-   After the download is complete, extract the zip file to a folder on
    your computer.

### Give Permission to Run Application

After extraction, open the extracted folder and double click on the file named
<img src="https://github.com/trendscenter/coinstac-instructions/blob/markdown/install-mac/media/image4.png" width="80" height="20"/>

You will be prompted with a warning that says this software is from an
unverified developer. This warning will only be issued once every time
you open a new version of COINSTAC. We have plans to remove it in the
future.

<img src="https://github.com/trendscenter/coinstac-instructions/blob/markdown/install-mac/media/image5.png" width="550" height="268"/>

You will have to do the following:

-   Click on the Apple icon 
<img src="https://github.com/trendscenter/coinstac-instructions/blob/markdown/install-mac/media/image6.png" width="20" height="20"/> 
in the top-left corner of your screen

-   Click System Preferences.

-   Click on Security & Privacy.

-   You will see a warning that coinstac was blocked because it was not from an identified developer.
    <img src="https://github.com/trendscenter/coinstac-instructions/blob/markdown/install-mac/media/image7.png" width="650" height="558"/> 


-   Click on the Open Anyway button

    -   If that does not work, do the following:

        -   Click on the lock in the lower left-hand corner.
        <img src="https://github.com/trendscenter/coinstac-instructions/blob/markdown/install-mac/media/image8.png" width="252" height="35"/> 

        -   Enter your password.

        -   Click on the Open Anyway button

        -   Close this window.

### Run Application

Next, go back to the folder where you extracted COINSTAC and double
click on the
<img src="https://github.com/trendscenter/coinstac-instructions/blob/markdown/install-mac/media/image4.png" width="82" height="22"/>  file again.
