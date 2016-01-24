#DJI Onboard SDK Windows QT Sample
##Intro
This example aims to help you understand and play with the basic flight procedures including:

* The Activation
* The Flight Control Obtainment
* The Flight control release
* The Take Off Procedure
* The Landing Procedure
* The Go Home Procedure
* The Attitude Control
* The Gimbal Control
* The Camera Control
* The Virtual RC Control
* The Waypoint Task Control

Developers can play with this example via the GUI interaction interface in Windows.


##Compile & Run Environment
The below environment are required.
* Qt Ver: QT 5.4  MinGW 32bit or later
* Compiler Ver: MinGW 4.9.2 or later; MSVC2012 32bit or later
  Note: MSVC-64bit is not supported, because the serial port driver in msvc only supports 32bit version, program will crash on 64bit compiler.


## Hardware Installation
* In order to communicate with the N1 Autopilot via the DJI OPEN protocal, a physical connection between your Onboard Device and the N1 Autopilot is required with a USB to TTL serial cable (SOLD Seperately).
* In order to monitor & control the flight, a remote controller connects to your Mobile Device (with the DJI GO APP running) is needed.

##Configs
1. Open *onboardSDK.pro* locates at *onboardSDK* sub-directory in *PureQT*.

2. Select a proper compiler and click *Configure Project* to proceed.

3. During the init process, enter the following info into the GUI interface including:

* APP ID
* Communication Key
* uart device name (e.g. COM1, COM2)
* baudrate

>Note: the 'baudrate' needs to be consistent with the setting in the DJI N1 PC assistant.

##Compile
Click the hammer icon on the bottom left in the Qt Creator IDE to start compiling.

##Run
Click the green triangle icon on the bottom left corner to run the sample.
We recommend you first run this example in the simulator then carefully move to the real flight test.

##What You Can Expect
* You can see the flight control simulations on screen if you are using the DJI PC simulator. Otherwise, real flight happens.
* You can see the actual 'gimbal and camera' movement.
* You can see the image/video you capture from you Mobile Device.
* You can start a groundstation task.

ENJOY your flight!