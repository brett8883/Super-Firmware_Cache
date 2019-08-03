=======================================================================================================

=== # CUSTOM MavicPro Brett8883 Personal Edition FLIGHT CONTROLLER MODULE===

Compiled by Brett8883 using Matoupi's FC_Patcher via Brett8883's Super-Patcher

**MUST be installed via Brett8883’s Super Patcher https://github.com/brett8883/DJI_Super-Patcher **

=======================================================================================================
Flight Controller Basic Info
=======================================================================================================

FLIGHT CONTROLLER COMMON NAME: MavicPro Brett8883 Personal Edition 

FILE NAME:MavicPro_brett8883_edition_wm220_0306_03.02.44.02_dji_system.bin

AIRCRAFT MODEL:MavicPro wm220

REQUIRED STOCK FW VERSION: v01.04.0300

FLIGHT CONTROLLER VERSION # 03.02.44.03

***WARNING: INCLUDESS PRE-MODIFIED PARAMETER VALUES!!***

-------------------------------------------------------------------------------------------------------

**Notes From the Author:**

This is the flight controller I personally use with the settings I fly with. WARNING some parameter values are set to dangerous values if not fully understood!
============================================================================================

**FC SUMMARY:**

Height limits disabled 

NFZ limits disabled 

GeoZone limits disabled 

Yaw speed min/max paramter ranges extended 

Galileo GPS Satellites reception enabled

Motors will start if inverted (if CSC at altitude and AC inverts the motors will start to save it)

Widened MIN/MAX vertical speed range in tripod mode

*******************************************************************************************

***Firmware Compatibility:***

To use this Custom firmware, your aircraft MUST BE ON STOCK FW: v01.04.0300

===

Know what you are doing before you use this.

********************************************************************************************

# WARNING THIS LIST IS INACCURATE. THIS LIST IS IN-PROGRESS UNDERCONTRUCTION 

*this list includes ALL paramters or parameter ranges that were changed even hardcoded values (galileo not config with parameters)*

**HEIGHT LIMIT DISABLED**
	
		"minValue" : 1,
		"maxValue" : 2,
		"defaultValue" : 2,
		"name" : "g_config.flying_limit.height_limit_enabled",
		"modify" : true
	
		"minValue" : 0.000000,
		"maxValue" : 100000.000000,
		"defaultValue" : 10000.000000,
		"name" : "g_config.flying_limit.limit_height_abs_without_gps"
	
		"minValue" : 0.000000,
		"maxValue" : 100000.000000,
		"defaultValue" : 10000.000000,
		"name" : "g_config.flying_limit.limit_height_abs"
	
		"minValue" : 0.000000,
		"maxValue" : 100000.000000,
		"defaultValue" : 10000.000000,
		"name" : "g_config.flying_limit.limit_height_rel"
	
**NFZ DISABLE**

		"minValue" : 0,
		"maxValue" : 1,
		"defaultValue" : 0,
		"name" : "g_config.airport_limit_cfg.cfg_enable[FLY_LIMIT_TYPE_SPECIAL]"

		"minValue" : 0,
		"maxValue" : 1,
		"defaultValue" : 0,
		"name" : "g_config.airport_limit_cfg.cfg_enable[FLY_LIMIT_TYPE_AIRPORT]"
		
		"minValue" : 0,
		"maxValue" : 4294967295,
		"defaultValue" : 20250910,
		"name" : "g_config.airport_limit_cfg.cfg_limit_data"

**GEOZONES DISABLED**

		"minValue" : 0,
		"maxValue" : 1,
		"defaultValue" : 0,
		"name" : "g_config.flying_limit.viechle_license_limit_enable"

		"minValue" : 0,
		"maxValue" : 1,
		"defaultValue" : 0,
		"name" : "g_config.flying_limit.driver_license_limit_enable"

		"maxValue" : 255,
		"defaultValue" : 1,
		"name" : "g_config.airport_limit_cfg.cfg_dis
		
		"minValue" : 0,
		"maxValue" : 65535,
		"defaultValue" : 1,
		"name" : "g_config.airport_limit_cfg.cfg_search_radius"
*********************************************************************************************************
		
**ENABLE MOTORS TO BE RESTARTED WHEN AIRCRAFT INVERTED**

		"minValue" : 0,
		"maxValue" : 1,
		"defaultValue" : 1,
		"name" : "g_cfg_debug.motor.no_start_motor_check"

		"minValue" : 0,
		"maxValue" : 1,
		"defaultValue" : 1,
		"name" : "g_config.fdi_open.close_auto_stop_motor_check"

*********************************************************************************************************
	
**Widened MIN/MAX Yaw speed range for P-GPS with OA sensors ON**

		"minValue" : 1.000000,
		"maxValue" : 200.000000,
		"defaultValue" : 30.000000,
		"name" : "g_config.avoid_cfg.avoid_tors_rate_range"

**Widened MIN/MAX Yaw speed range for P-GPS with OA sensors OFF**

		
		"minValue" : 1.000000,
		"maxValue" : 250.000000,
		"defaultValue" : 35.000000,
		"name" : "g_config.mode_normal_cfg.tors_gyro_range"
		
**Widened MIN/MAX Yaw speed range for beginner mode**

		"minValue" : 1.000000,
		"maxValue" : 300.000000,
		"defaultValue" : 70.000000,
		"name" : "g_config.mode_gentle_cfg.tors_gyro_range"

**Widened MIN/MAX Yaw speed range for sport mode. Slowed max yaw speed in Sport mode**

		"minValue" : 1.000000,
		"maxValue" : 300.000000,
		"defaultValue" : 35.000000,
		"name" : "g_config.mode_sport_cfg.tors_gyro_range"
	
**Widened MIN/MAX Yaw speed range for prop cage mode**

		"minValue" : 1.000000,
		"maxValue" : 250.000000,
		"defaultValue" : 90.000000,
		"name" : "g_config.prop_cover_cfg.tors_gyro_range"
		
**Widened MIN/MAX Yaw speed range for Cinematic mode**

		"index" : 760,
		"typeID" : 8,
		"size" : 4,
		"attribute" : 14,
		"minValue" : 1.000000,
		"maxValue" : 250.000000,
		"defaultValue" : 50.000000,
		"name" : "CM_tors_range"
	
**Widened MIN/MAX Yaw speed range for tripod mode**

		"minValue" : 1.000000,
		"maxValue" : 300.000000,
		"defaultValue" : 15.000000,
		"name" : "g_config.mode_tripod_cfg.tors_gyro_range"
		
**Widened MIN/MAX Yaw speed range for manual mode**

		"minValue" : 1.000000,
		"maxValue" : 500.000000,
		"defaultValue" : 150.000000,
		"name" : "g_config.mode_manual_cfg.tors_gyro_range"
	
**Widened MIN/MAX Yaw speed range for waypoint mode**

		"minValue" : 1.000000,
		"maxValue" : 300.000000,
		"defaultValue" : 90.000000,
		"name" : "g_config.waypoint_cfg.max_auto_yaw_rate"
		
*********************************************************************************
**Widened MIN/MAX vertical speed range in tripod mode**
 
		"minValue" : 0.500000,
		"maxValue" : 10.000000,
		"defaultValue" : 1.000000,
		"name" : "g_config.mode_tripod_cfg.vert_vel_up"
	
		"minValue" : -10.000000,
		"maxValue" : -0.500000,
		"defaultValue" : -1.000000,
		"name" : "g_config.mode_tripod_cfg.vert_vel_down"

**Increase Attitude Range Availible to Pilot in P-GPS mode with OA sensors on**

- Also increased range this value can be configured with 

		"minValue" : 0.100000,
		"maxValue" : 1.000000,
		"defaultValue" : 0.800000,
		"name" : "g_config.avoid_cfg.avoid_rc_scale"

**Increased max attitude angle(aka speed) with OA sensors on**


		"minValue" : 10.000000,
		"maxValue" : 60.000000,
		"defaultValue" : 30.000000,
		"name" : "g_config.avoid_cfg.avoid_atti_range"

		"minValue" : 10,
		"maxValue" : 60,
		"defaultValue" : 16,
		"name" : "g_config.control.avoid_atti_range"

**Reduced the start/stop sensitivity of rc sticks on the yaw axis of the aircraft**

		"minValue" : 1,
		"maxValue" : 100,
		"defaultValue" : 10,
		"name" : "yaw_sensitive_gain"
		
**Reduced throttle sensitivity**

		"minValue" : 1,
		"maxValue" : 100,
		"defaultValue" : 50,
		"name" : "g_config.control.rc_throttle_sensitivity"

**Slowed tilt sensitivity on the elevator**
		
		"minValue" : 1,
		"maxValue" : 100,
		"defaultValue" : 50,
		"name" : "tilt_sensitive_gain"

**WARNING!! POTENTIALLY DANGEROUS VALUE!**	
	
Decreased brake gain to 10 and increased possible range of brake vaules. Will take a long time to slow to a stop. USE CAUTION!
	
		"minValue" : 1,
		"maxValue" : 200,
		"defaultValue" : 10,
		"name" : "brake_sensitive_gain"
		
Increased attitude range availible to the pilot with the elevator in sport mode

		"maxValue" : 10.00000,
		"defaultValue" : 0.950000,
		"name" : "g_config.mode_sport_cfg.rc_scale"

Increased possible attitude range in sport mode (default value remains factory default,did not change the default value)

		"minValue" : 10.000000,
		"maxValue" : 100.000000,
		"defaultValue" : 35.000000,
		"name" : "g_config.mode_sport_cfg.tilt_atti_range"

Increased vertical speed up in Sport mode

		"minValue" : 1.000000,
		"maxValue" : 10.000000,
		"defaultValue" : 6.000000,
		"name" : "g_config.mode_sport_cfg.vert_vel_up"

WARNING!! POTENTIALLY DANGEROUS VALUE!
Increased vertical speed down in Sport mode. Full throttle down is about 20mph! **CAUTION**
		"minValue" : -10.000000,
		"maxValue" : -1.000000,
		"defaultValue" : -9.000000,
		"name" : "g_config.mode_sport_cfg.vert_vel_down"


		"minValue" : 10.000000,
		"maxValue" : 1000.000000,
		"defaultValue" : 30.000000,
		"name" : "g_config.mode_normal_cfg.tilt_atti_range"

WARNING!! POTENTIALLY DANGEROUS VALUE!

	-Disabled auto-land due to low battery

		"minValue" : 0,
		"maxValue" : 1,
		"defaultValue" : 0,
		"name" : "g_config.bat_config.enable_smart_bat_landing_portect"

WARNING!! POTENTIALLY DANGEROUS VALUE!

	- Decresed battery warning levels. Widened range of possible battery warning levels that can be configured

		
		"minValue" : 1,
		"maxValue" : 100,
		"defaultValue" : 10,
		"name" : "dji_bat_level_1"
	
		"minValue" : 1,
		"maxValue" : 100,
		"defaultValue" : 5,
		"name" : "dji_bat_level_2"
		
Enabled Sport mode by default. Factory settings required Sport mode to be activaated using the "enable multiple modes in DJI Go 4. This is enabled by defualt with this flight controller

		"minValue" : 0,
		"maxValue" : 1,
		"defaultValue" : 1,
		"name" : "enable_multiple_mode"


		
		
		
		
		
		
		