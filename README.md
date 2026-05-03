
# 3DR Solo RubyFPV Conversion

This is a log of my adventure converting the SOLO link used in the 3dr solo drones to being used with RubyFPV over the old method that leveraged 3DR's own software which was updated by the OpenSolo Project. The eventual goal is to essentially recreate the SOLO Link using the new ideas RubyFPV has created for a more versitile videolink with some changes made for my use case. The eventual goal is to use the 3DR controller to get live telemetry from the Drone along with a live HD video link to be used to control the gimbal by a seprate operator and use an alternative control link (ELRS most likely) for the main operator controlling the rest of the drone. 


## Roadmap
### Drone and Controller
- [ ] Get RubyFPV working on both drone and controller
    - [ ] Get RubyFPV running on either the drone or controller side IMX6
        - [ ] Get existing PCIe WiFi cards identified and accessable by RubyFPV
            - [ ] Use known working USB WiFi chipsets
    - [ ] Swap IMX6 with RPI on drone and Radxa in controller with known working USB chipsets
- [ ] Get live video feed from HDMI input on drone and output on controller HDMI
- [ ] Get Mavlink telemetry working over RubyFPV and BiDirectional communication with the black cube flight controller
### Controller
- [ ] Integrate 3DR Solo controller via USB or Serial for controlling drone over BiDirectional Mavlink
- [ ] Reuse 3DR Solo controller for display 
    - [ ] Controller Battery Level
    - [ ] Drone Battery Level
    - [ ] Flight Stats
    - [ ] Communication Link
    - [ ] Party Tricks????
- [ ] External serial/USB interface for Mavlink telemetry for use with MissionPlanner, QGroundControl, ETC
