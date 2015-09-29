## MAVinline

* Control by MAVProxy


### All commands

* accelcal             : do 3D accelerometer calibration
* ahrstrim             : do AHRS trim
* alias                : command aliases
* alt                  : show altitude information
* arm                  : arm motors
* auxopt               : select option for aux switches on CH7 and CH8 (ArduCopter only)
* bat                  : show battery information
* calpress             : calibrate pressure sensors
* camctrlmsg           : camctrlmsg
* cammsg               : cammsg
* changealt            : change target altitude
* compassmot           : do compass/motor interference calibration
* disarm               : disarm motors
* fence                : geo-fence management
* ground               : do a ground start
* guided               : fly to a clicked location on map
* gyrocal              : do gyro calibration
* land                 : auto land
* level                : set level on a multicopter
* link                 : link control
* log                  : log file handling
* magcal               : magcal
* mode                 : mode change
* module               : module commands
* motortest            : motortest commands
* output               : output control
* param                : parameter handling
* rally                : rally point control
* rc                   : RC input control
* rcbind               : bind RC receiver
* reboot               : reboot autopilot
* relay                : relay commands
* repeat               : repeat a command at regular intervals
* reset                : reopen the connection to the MAVLink master
* script               : run a script of MAVProxy commands
* servo                : servo commands
* set                  : mavproxy settings
* setspeed             : do_change_speed
* setup                : go into setup mode
* setyaw               : condition_yaw
* shell                : run shell command
* status               : show status
* switch               : flight mode switch control
* takeoff              : takeoff
* terrain              : terrain control
* time                 : show autopilot time
* tuneopt              : Select option for Tune Pot on Channel 6 (quadcopter only)
* up                   : adjust pitch trim by up to 5 degrees
* velocity             : velocity
* version              : show version
* watch                : watch a MAVLink pattern
* wp                   : waypoint management

### Status

> The data returns from `status` commend is comes from `mpstate.status.msgs`.

They are:
* `VFR_HUD`
* `ATTITUDE`
* `HEARTBEAT`
* `MISSION_CURRENT`
* `RAW_IMU`
* `GPS_RAW_INT`
* `SCALED_IMU2`
* `NAV_CONTROLLER_OUTPUT`
* `VFR_HUD`
* `MEMINFO`
* `HWSTATUS`
* `STATUSTEXT`
* `BAD_DATA`
* `SENSOR_OFFSETS`
* `AHRS`
* `SCALED_PRESSURE`
* `GLOBAL_POSITION_INT`,
* `SYS_STATUS`,
* `POWER_STATUS`
* `PARAM_VALUE`
* `SYSTEM_TIME`
* `SERVO_OUTPUT_RAW`
* `RC_CHANNELS_RAW`

Maybe more...

### RC

> Using `RC` commend is a way to control the copter. The channel value is 1100 ~ 1950(RC1~RC8), get the current values by `status RC_CHANNELS_RAW`

* channel 1: -
* channel 2: -
* channel 3: -
* channel 4: -
* channel 5: -
* channel 6: -
* channel 7: -
* channel 8: -

```json
{'chan1_raw' : 1521, 'chan2_raw' : 1521, 'chan3_raw' : 1100, 'chan4_raw' : 1950, 'chan5_raw' : 1521, 'chan6_raw' : 1519, 'chan7_raw' : 1520, 'chan8_raw' : 1521}
```