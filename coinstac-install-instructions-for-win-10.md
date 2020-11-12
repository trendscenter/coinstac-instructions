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

Below are instructions for how to set up COINSTAC on your computer. The
following steps should be taken, which are explained below:

1.  Verify System Requirements

2.  Install Docker

3.  Download and Run COINSTAC Application

Verify System Requirements
--------------------------

Use a Windows 10 Professional 64-bit computer that has at least 8 GB of
memory. As of this writing, Windows 10 Home edition will not work.

Install Docker
--------------

### Installation

Log into an account with Administrator privileges and install Docker
Community Edition for Windows using one of the below methods.

#### Standard Installation

Install Docker using these instructions:

[https://store.docker.com/editions/community/docker-ce-desktop-windows](https://store.docker.com/editions/community/docker-ce-desktop-windows)

#### Using WSL 2 Backend (alternative)

Alternatively, you can install Docker using the WSL 2 backend by following these instructions:

[https://docs.docker.com/docker-for-windows/wsl/](https://docs.docker.com/docker-for-windows/wsl/)

Note that this may give you a better experience with Docker, but it has not been tested with COINSTAC yet.

### Verify Installation

Check that docker is installed by opening a Powershell window and
typing:

### Run Application

You should see a similar message, probably with a different version and
build:

> Docker version 18.03.1-ce, build 9ee9f40

### Give Privileges to Accounts Without Administrator Privileges

If you want to run COINSTAC on another account without Administrator
privileges, then do the following:

1.  Close Docker

2.  Search for Windows Computer Management in the search box on the left
    side of your taskbar.

3.  Run Windows Computer Management as an Administrator. You should see this window.
    <img src="https://github.com/trendscenter/coinstac-instructions/blob/markdown/install-win/media/image1.png" width="650" height="690"/> 

4.  Click on System Tools and then Local Users and
    Groups
    <img src="https://github.com/trendscenter/coinstac-instructions/blob/markdown/install-win/media/image2.png" width="650" height="690"/> 

5.  Right click the **docker-users** group and click \"Add to
    Group\...\"

6.  A dialog box called \"docker-users Properties\" will
    appear.
    <img src="https://github.com/trendscenter/coinstac-instructions/blob/markdown/install-win/media/image3.png" width="650" height="739"/> 

7.  Click \"Add\...\"

8.  Click \"Advanced\...\"

9.  Make sure \"Select this object type:\" is set to \"Users or Built-in
    security principals\"

10. Click \"Find Now\"

11. Select the user account on which you want to run
    COINSTAC
    <img src="https://github.com/trendscenter/coinstac-instructions/blob/markdown/install-win/media/image4.png" width="650" height="731"/> 

12. Click OK

13. Click OK

14. Click OK

15. Add the same user to Hyper-V Administrators using the same method described above (steps 5-14).

16. Exit from Windows Computer Management.

17. Sign out of the Administrator account.

18. Sign out of the account with which you want to run COINSTAC for the group permissions changes to take effect.

19. Sign back into the account without Administrator privileges and run Docker for Windows.

### Running Docker

To run Docker on Windows:

-   Enter \"docker\" into the search prompt on your taskbar. This will bring up Docker for Windows as the best match.

-   Click on Docker for Windows.

### Possible Docker Errors

#### Possible Error \#1

After installing Docker on Windows 10, you may see the following error.

    <img src="https://github.com/trendscenter/coinstac-instructions/blob/markdown/install-win/media/image5.png" width="570" height="213"/> 

To fix this error, you will need to enable virtualization on your
computer\'s BIOS. Follow this
[guide](https://blogs.technet.microsoft.com/canitpro/2015/09/08/step-by-step-enabling-hyper-v-for-use-on-windows-10/)
to accomplish that. To get to the BIOS on Windows 10, you can use this
[guide](https://www.laptopmag.com/articles/access-bios-windows-10).

#### Possible Error \#2

You may also get this error when you launch Docker or run COINSTAC:

> Docker hv-sock proxy (vsudd) is not reachable
>
> at Docker.Core.Pipe.NamedPipeClient.Send(String action, Object\[\]
> parameters) in
> C:\\gopath\\src\\[github.com](http://github.com/)\\docker\\pinata\\win\\src\\Docker.Core\\pipe\\NamedPipeClient.cs:line
> 36
>
> at Docker.Actions.DoStart(SynchronizationContext syncCtx, Boolean
> showWelcomeWindow, Boolean executeAfterStartCleanup) in
> C:\\gopath\\src\\[github.com](http://github.com/)\\docker\\pinata\\win\\src\\Docker.Windows\\Actions.cs:line
> 67
>
> at Docker.Actions.\<\>c\_\_DisplayClass14\_0.\<Start\>b\_\_0() in
> C:\\gopath\\src\\[github.com](http://github.com/)\\docker\\pinata\\win\\src\\Docker.Windows\\Actions.cs:line
> 51
>
> at Docker.WPF.TaskQueue.\<\>c\_\_DisplayClass19\_0.\<.ctor\>b\_\_1()
> in
> C:\\gopath\\src\\[github.com](http://github.com/)\\docker\\pinata\\win\\src\\Docker.WPF\\TaskQueue.cs:line
> 59

To fix this error:

-   Click on Show Hidden Icons (\^) on your taskbar. You\'ll see a group
    of small icons.

-   Right click on the Docker icon <img src="https://github.com/trendscenter/coinstac-instructions/blob/markdown/install-win/media/image6.png" width="29" height="29"/> 

-   Click on Settings.

-   Click Reset and then Reset to Factory Defaults. A window will appear
    asking if you are sure you want to reset.

-   Click the Reset button.

### Verify Docker is Running

Before starting COINSTAC, verify that Docker is running on your computer
by using one of the methods below.

#### Method \#1

You can verify that Docker is running by hovering over the Docker icon <img src="https://github.com/trendscenter/coinstac-instructions/blob/markdown/install-win/media/image6.png" width="29" height="29"/> 
on your taskbar. You should see a message that Docker is running.

#### Method \#2

Open a Powershell window and type:

> docker ps

You should see an output like this:

> CONTAINER ID IMAGE COMMAND CREATED STATUS PORTS NAMES

If you see an error message, then you have to start Docker.

Download and Run COINSTAC Application
-------------------------------------

### Download

To download the COINSTAC application, go to this page and download the
latest release:

[https://github.com/MRN-Code/coinstac/releases/](https://github.com/MRN-Code/coinstac/releases/)

-   Download the file named **coinstac-win32-x64.zip**.

-   After the download is complete, extract the zip file to a folder on
    your computer.

### Give Permission to Run Application

After extraction, open the extracted folder and double click on the file
named <img src="https://github.com/trendscenter/coinstac-instructions/blob/markdown/install-win/media/image7.png" width="82" height="22"/> 

You\'ll see this window warning you about an unrecognized app. This
warning will only be issued once every time you open a new version of
COINSTAC.

<img src="https://github.com/trendscenter/coinstac-instructions/blob/markdown/install-win/media/image8.png" width="288" height="267"/> 

-   Click More Info

-   Click Run anyway

### Run Application

After you have given your computer permission to run the application,
double click on the <img src="https://github.com/trendscenter/coinstac-instructions/blob/markdown/install-win/media/image7.png" width="82" height="22"/> 

Docker will ask you to enable Hyper-V and Container features. Enable
those features. Do not click on the button to enable using Windows
containers.

### Docker Drive Permissions

When you run a pipeline for the first time, you will be prompted to
share data with Docker on your computer. Pick the drives that contain
the data you want to use with COINSTAC or on which you will run COINSTAC
(usually at least C drive). You\'ll have to enter your password to
complete this step.
