### Simu5G Installation:

-   Download the Simu5G tarball ([zip](https://github.com/Unipisa/Simu5G/archive/refs/tags/v1.1.0.zip),  [tar.gz](https://github.com/Unipisa/Simu5G/archive/refs/tags/v1.1.0.tar.gz)) including the latest  _stable release_. This version requires  _OMNeT++ v5.6.2_  and  _INET v4.2.2_;


####  Prerequisites
Simu5G can be compiled on any platform supported by OMNeT++ and NET frameworks.

You should have working  [OMNeT++](http://omnetpp.org/)  and  [INET Framework](http://inet.omnetpp.org/)  installations. See the required versions above, depending on the Simu5G version you selected (latest stable release is used in this repository).

:warning: Make sure your OMNeT++ installation works OK.

:warning: Install and test INET according to the installation instructions found in the archive. Be sure to check if the INET examples are running fine before continuing.


#### Building Simu5G from IDE:


 1.  Extract the downloaded Simu5G tarball next to the "inet4" directory (i.e. into your workspace directory, if you are using the IDE).
2.  Start the IDE, and ensure that the 'inet' project is open and correctly built.
3.  Import the project using: File | Import | General | Existing projects into Workspace. Then select the workspace dir as the root directory, and be sure NOT to check the "Copy projects into workspace" box. Click Finish.
4.  You can build the project by pressing CTRL-B (Project | Build all)
5.  To run an example from the IDE, select the simulation example's folder under 'simulations', and click 'Run' on the toolbar.

#### Building Simu5G from the command line:


 1.  Extract the downloaded Simu5G tarball next to the "inet4" directory
2.  Change to the Simu5G directory.
3.  Type ". setenv". This will add the Simu5g/bin directory to the PATH environment variable.
4.  Type "make makefiles". This should generate the makefiles.
5.  Type "make" to build the Simu5G executable (debug version). Use "make MODE=release" to build release version.
6.  Run an examples by changing into one of the directories under 'simulations/NR', and executing "./run"

#### Troubleshooting: 
:bulb: After importing the Simu5G to OmNet++, you should change the preferences with "**inet**" from "**inet4**". 

:bulb: Make sure that you have run "`. setenv`" in the `/bin` directory, if you follow the building Simu5G from IDE.
