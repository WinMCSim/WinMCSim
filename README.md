# WinMCSim
GNU MCSim for Microsoft Windows

Refer to [the GNU MCSim web site](https://www.gnu.org/software/mcsim/) for more information about MCSim and how to use it.

## Prerequisites
* Microsoft Windows 7 SP1 or later
* R 3.1+ (optional)

Please note that the installer for WinMCSim will install Microsoft .NET 4.6.2 if it is not already present on the target system. 

## Build Tools
To build an simulation executable, MCSim makes use of a C++ compiler. WinMCSim requires the 2017 version of Microsoft Visual C++ (MSVC) to be installed on the target system. The user has the option to install MSVC manually, or to make use of the installer provided with WinMCSim. **Warning!** Installation of MSVC will consume around 2GB of disk space.

### Manual Installation of MSVC 2017
Download _Build Tools for Visual Studio 2017_ from [Visual Studio Downloads](https://www.visualstudio.com/downloads/). Run the installer and select the workload for _Visual C++ build tools_. All **required** and **recommended** components listed in the [component directory for Visual C++ build tools workload](https://docs.microsoft.com/en-gb/visualstudio/install/workload-component-id-vs-build-tools#visual-c-build-tools) must be installed.  

### Build Tools Installer for WinMCSim
After WinMCSim has been installed, launch _SimBuildTools_ from the _Start_ menu. SimBuildTools employs [PowerShell](https://docs.microsoft.com/en-us/powershell/) and [Chocolatey](https://chocolatey.org/packages/visualstudio2017-workload-vctools) to partly automate installation of MSVC. Use of these tools requires local administrator access to the target system. At start-up SimBuildTools will request permission from the user to run at elevated privilege. Once started, simply complete the three steps in the order shown. **Warning!** Depending on the speed both of the user's Internet connection and of the target system, the third step, which installs the MSVC workload, may require a considerable period to complete (allow for several hours).

## Download
Download an installer for the latest build of WinMCSim from [releases](http://www.github.com/HSL/WinMCsim/releases/).
