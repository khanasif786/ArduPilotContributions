# ArduPilotContributions
### AP_Proximity: Removed AP_Proximity_LightWareSF40C_v09
Deleted older drivers for fixing running out of flash space in some boards.

### [AP_GyroFFT: fix 'arm_status' shadowing a global declaration error](https://github.com/ArduPilot/ardupilot/pull/20075)
Mavlink bindings generated from AVSUAS xml shadows 'arm_status' causing error.

### Autotest: Copter test fix for tri frame
Fixed excessive yaw rate of 'tri' frame. Using default copter params.

### Plane: add support for MAV_CMD_DO_AUTOTUNE by Axis
PR for adding support for  MAV_CMD_DO_AUTOTUNE_ENABLE  that allows the GCS to specify the axes as a bitmask in param2.

### Plane: Max altitude for FBWB (Currently In work)
Maximum altitude in centimeters or meters that FBWB, and CRUISE modes will allow. If you attempt to ascend above this altitude, then the plane will level off. A value of zero means no limit.
