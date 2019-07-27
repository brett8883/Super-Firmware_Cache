# CUSTOM DJI MavicPro/Platinum Stealth Variant

Compiled by Brett8883 using Matoupi's FC_Patcher via Brett8883's Super-Patcher

**MUST be installed via Brett8883’s Super Patcher https://github.com/brett8883/DJI_Super-Patcher **

=======================================================================================================
=======================================================================================================
AIRCRAFT MODEL:MavicPro/Platinum 

REQUIRED STOCK FW VERSION: v01.04.0300

FLIGHT CONTROLLER version # 03.02.44.97

-------------------------------------------------------------------------------------------------------

FC SUMMARY:

Height limits disabled 

NFZ limits disabled 

GeoZone limits disabled 

Yaw speed min/max paramter ranges extended 

Galileo GPS Satellites reception enabled

Motors will start if inverted (if CSC at altitude and AC inverts the motors will start to save it)

Widened MIN/MAX vertical speed range in tripod mode

rear light is switched to off while in flight 

*******************************************************************************************

Notes From the Author:

• Standard Super Patcher Custom Flight Controller modifications 

• Rear AC light is programmed to remain off while in flight. WARNING THIS CANNOT BE CHANGED BY USER!
To turn the light back on the user would need to flash a stock version of 01.04.0300 to uninstall

Rear LED parameter is hard coded so this change cannot be undone is Assistant 2 1.1.2. A FC reflash is required to undo. 

Note: rear light will activate during start up and may also turn on if an aircraft error is present. This includes critical low battery

============================================================================================

***Firmware Compatibility:***

To use this Custom firmware, your aircraft MUST BE ON STOCK FW: V01.04.0300 or already be on another Super-Patcher Variant with a different FC#. 

**When in doubt flash stock V01.04.0300**


===

Know what you are doing before you use this.

********************************************************************************************

Full Change Log for Super-Patcher **Mavic Pro Stealth** Variant Custom Flight Controller

*this list includes ALL paramters or parameter ranges that were changed even hardcoded values (galileo not config with parameters)

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
	
NFZ DISABLE

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

GEOZONES DISABLED

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
		
ENABLE MOTORS TO BE RESTARTED WHEN AIRCRAFT INVERTED

		"minValue" : 0,
		"maxValue" : 1,
		"defaultValue" : 1,
		"name" : "g_cfg_debug.motor.no_start_motor_check"

		"minValue" : 0,
		"maxValue" : 1,
		"defaultValue" : 1,
		"name" : "g_config.fdi_open.close_auto_stop_motor_check"

*********************************************************************************************************
	
Widened MIN/MAX Yaw speed range for P-GPS with OA sensors ON

		"minValue" : 1.000000,
		"maxValue" : 200.000000,
		"defaultValue" : 70.000000,
		"name" : "g_config.avoid_cfg.avoid_tors_rate_range"

{Widened MIN/MAX Yaw speed range for P-GPS with OA sensors OFF

		"minValue" : 1.000000,
		"maxValue" : 300.000000,
		"defaultValue" : 90.000000,
		"name" : "g_config.mode_normal_cfg.tors_gyro_range"

{Widened MIN/MAX Yaw speed range for beginner mode

		"minValue" : 1.000000,
		"maxValue" : 300.000000,
		"defaultValue" : 70.000000,
		"name" : "g_config.mode_gentle_cfg.tors_gyro_range"

Widened MIN/MAX Yaw speed range for sport mode

		"minValue" : 1.000000,
		"maxValue" : 300.000000,
		"defaultValue" : 150.000000,
		"name" : "g_config.mode_sport_cfg.tors_gyro_range"
	
Widened MIN/MAX Yaw speed range for prop cage mode

		"minValue" : 1.000000,
		"maxValue" : 250.000000,
		"defaultValue" : 90.000000,
		"name" : "g_config.prop_cover_cfg.tors_gyro_range"
		
Widened MIN/MAX Yaw speed range for Cinematic mode

		"index" : 760,
		"typeID" : 8,
		"size" : 4,
		"attribute" : 14,
		"minValue" : 1.000000,
		"maxValue" : 250.000000,
		"defaultValue" : 50.000000,
		"name" : "CM_tors_range"
	
{Widened MIN/MAX Yaw speed range for tripod mode

		"minValue" : 1.000000,
		"maxValue" : 300.000000,
		"defaultValue" : 15.000000,
		"name" : "g_config.mode_tripod_cfg.tors_gyro_range"
		
{Widened MIN/MAX Yaw speed range for manual mode

		"minValue" : 1.000000,
		"maxValue" : 500.000000,
		"defaultValue" : 150.000000,
		"name" : "g_config.mode_manual_cfg.tors_gyro_range"
	
Widened MIN/MAX Yaw speed range for waypoint mode 

		"minValue" : 1.000000,
		"maxValue" : 300.000000,
		"defaultValue" : 90.000000,
		"name" : "g_config.waypoint_cfg.max_auto_yaw_rate"
		
*********************************************************************************

Widened MIN/MAX vertical speed range in tripod mode
 
		"minValue" : 0.500000,
		"maxValue" : 10.000000,
		"defaultValue" : 1.000000,
		"name" : "g_config.mode_tripod_cfg.vert_vel_up"
	
		"minValue" : -10.000000,
		"maxValue" : -0.500000,
		"defaultValue" : -1.000000,
		"name" : "g_config.mode_tripod_cfg.vert_vel_down"

*********************************************************************************

Turn off rear LED during flight 	

		"minValue" : 0,
		"maxValue" : 1,
		"defaultValue" : 0,
		"name" : "g_cfg_debug.force_flash_led"
**********************************************************************************
See flyc_param_infos file for all parameters with their min/max and default values. This file includes hard-coded values. 
