# ArduPilotContributions
Only flightstack contributions are here-
### [AP_Proximity: Removed AP_Proximity_LightWareSF40C_v09](https://github.com/ArduPilot/ardupilot/pull/19707)
- Deleted older drivers for fixing running out of flash space in some boards.

### [AP_GyroFFT: fix 'arm_status' shadowing a global declaration error](https://github.com/ArduPilot/ardupilot/pull/20075)
- Mavlink bindings generated from AVSUAS xml shadows 'arm_status' causing error.

### [Autotest: Copter test fix for tri frame](https://github.com/ArduPilot/ardupilot/pull/19674)
- Fixed excessive yaw rate of 'tri' frame. Using default copter params.

### [Plane: add support for MAV_CMD_DO_AUTOTUNE by Axis](https://github.com/ArduPilot/ardupilot/pull/19742)
- PR for adding support for  MAV_CMD_DO_AUTOTUNE_ENABLE  that allows the GCS to specify the axes as a bitmask in param2.

### [Plane: Max altitude for FBWB](https://github.com/ArduPilot/ardupilot/pull/19732) 
- (work in progress)
Maximum altitude in centimeters or meters that FBWB, and CRUISE modes will allow. If you attempt to ascend above this altitude, then the plane will level off. A value of zero means no limit.

### [Added compass glitch detection to fix gps_glitch showing in mag anomaly #20605](https://github.com/ArduPilot/ardupilot/pull/20605)
- fixes EKF: "GPS Glitch" warning can be misleading because it's not always the GPS that is misbehaving.

### [removed yaw_rate args from set_target_angle_and_climbrate #20436](https://github.com/ArduPilot/ardupilot/pull/20436)
- Newer version of this pull [fixed set_target_angle_and_climbrate's use_yaw_rate fields don't work](https://github.com/ArduPilot/ardupilot/pull/20435)

### [AP_Scripting: changed MAV_SEVERITY_EMERGENCY to INFO for origin set #20739](https://github.com/ArduPilot/ardupilot/pull/20739)
- Changed MAV_SEVERITY_EMERGENCY to MAV_SEVERITY_INFO for origin set command ack message on GCS.
