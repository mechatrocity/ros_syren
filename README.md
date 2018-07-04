# ros_syren
ROS driver for the SyRen 10 and SyRen 25 motor drivers.  See the [SyRen user's guide](https://www.dimensionengineering.com/datasheets/SyRen10-25.pdf). 

### Supported Platforms
Originally targeting the Arduino and Beaglebone (Black) platforms.

## Hardware Interface
Two output lines on the Robot computer are needed in order to interface with a SyRen, one to transmit serial data (connects to S1), and an active-low Emergency Stop signal (connects to S2)  

### Packetized Serial
The SyRen should be configured for Operating Mode 4: Packetized serial.

This appears to be, by far, the 'safest" of the four operating mode; the SyRen will perform a checksum integrity check on incoming data, it includes commands to configure minimum and maximum battery voltage levels for operation, and it includes a dedicated E-stop channel.

## ROS Interface
<TODO> standard ROS-style of documenting this...

### Subscribers
* <TODO> Drive Command

### Services
* <TODO> E-stop Request
* <TODO> Set minimum battery voltage
* <TODO> Set maximum battery voltage
