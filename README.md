## MAVinline

* Control by MAVProxy

### status

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

* channel 1: 
* channel 2: 
* channel 3: velocity
* channel 4: 
* channel 5: 
* channel 6: 
* channel 7: 
* channel 8: 

```json
{chan1_raw : 1521, chan2_raw : 1521, chan3_raw : 1100, chan4_raw : 1950, chan5_raw : 1521, chan6_raw : 1519, chan7_raw : 1520, chan8_raw : 1521}
{chan1_raw : 1521, chan2_raw : 1520, chan3_raw : 1100, chan4_raw : 1950, chan5_raw : 1520, chan6_raw : 1520, chan7_raw : 1520, chan8_raw : 1521}
```