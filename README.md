# w10m-emulator-template

Getting Windows 10 Mobile emulator running on Visual Studio 2017 Community is a bit finicky. This is how I got it to work as of 18 August 2018.

Steps to reproduce:

1. Download and install [Visual Studio 2017 Community edition](https://visualstudio.microsoft.com/vs/community/).
1. Install the following dependencies:
    1. In Visual Studio Installer under the Workloads tab select:
        - `The Universal Windows Platform development` Workload
    1. Then under the Individual components tab select all of the following:
        - `Windows 10 Mobile Emulator (Creators Update)`
        - `Windows 10 Mobile Emulator (Fall Creators Update)`
        - `Windows 10 SDK 10.0.15063.0`
        - `Windows 10 SDK 10.0.16299.0`
    1. Click Install/Modify, wait for packages to install, and reboot if necessary (to enable Hyper-V).
    1. Optionally you can also install:
        - [Mobile Emulator Insider Preview](https://www.microsoft.com/en-us/software-download/windowsinsiderpreviewSDK)
1. Download and extract a [.zip file](https://github.com/sirredbeard/w10m-emulator-template/archive/master.zip) of this repository.
1. Open w10m-emulator-template.sln in Visual Studio 2017.
1. Set platform to x86 or x64, as applicable.
1. Select preferred emulator image from the drop-down box, see:

<img src="https://raw.githubusercontent.com/sirredbeard/w10m-emulator-template/master/Capture.PNG">

Run.