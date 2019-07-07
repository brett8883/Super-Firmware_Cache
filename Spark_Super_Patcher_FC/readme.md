====CUSTOM DJI SPARK FLIGHT CONTROLLER MODULE====

Compiled by Brett8883 using Matoupi's FC_Patcher via Brett8883's Super-Patcher

**MUST be installed via Brett8883’s Super Patcher https://github.com/brett8883/DJI_Super-Patcher **

===
FLIGHT CONTROLLER version # 03.02.44.09

Height limits disabled 

NFZ limits disabled 

GeoZone limits disabled 

Yaw speed min/max paramter ranges extended 

Galileo GPS Satellites reception enabled




===

Notes From the Author:
• 
===

***Firmware Compatibility:***

To use this Custom firmware, your DJI Spark MUST BE ON STOCK FW v01.00.0900

===

Know what you are doing before you use this.
********************************************************************************************

Full Change Log for Super-Patcher Standard Spark DJI Super-Patcher Custom Flight Controller

*this list includes ALL paramters that were changed even hardcoded values (galileo not config with parameters)

HEIGHT LIMIT DISABLED
	{
		"index" : 5,
		"typeID" : 0,
		"size" : 1,
		"attribute" : 43,
		"minValue" : 1,
		"maxValue" : 2,
		"defaultValue" : 2,
		"name" : "g_config.flying_limit.height_limit_enabled",
		"modify" : true
	},
{
		"index" : 204,
		"typeID" : 8,
		"size" : 4,
		"attribute" : 51,
		"minValue" : 0.000000,
		"maxValue" : 100000.000000,
		"defaultValue" : 10000.000000,
		"name" : "g_config.flying_limit.limit_height_abs_without_gps"
	},
{
		"index" : 203,
		"typeID" : 8,
		"size" : 4,
		"attribute" : 39,
		"minValue" : 0.000000,
		"maxValue" : 100000.000000,
		"defaultValue" : 10000.000000,
		"name" : "g_config.flying_limit.limit_height_abs"
	},{
		"index" : 202,
		"typeID" : 8,
		"size" : 4,
		"attribute" : 39,
		"minValue" : 0.000000,
		"maxValue" : 100000.000000,
		"defaultValue" : 10000.000000,
		"name" : "g_config.flying_limit.limit_height_rel"
	},
NFZ DISABLE
{
		"index" : 1107,
		"typeID" : 0,
		"size" : 1,
		"attribute" : 62,
		"minValue" : 0,
		"maxValue" : 1,
		"defaultValue" : 0,
		"name" : "g_config.airport_limit_cfg.cfg_enable[FLY_LIMIT_TYPE_SPECIAL]"
{
		"index" : 1106,
		"typeID" : 0,
		"size" : 1,
		"attribute" : 62,
		"minValue" : 0,
		"maxValue" : 1,
		"defaultValue" : 0,
		"name" : "g_config.airport_limit_cfg.cfg_enable[FLY_LIMIT_TYPE_AIRPORT]"
		
{
		"index" : 2,
		"typeID" : 2,
		"size" : 4,
		"attribute" : 42,
		"minValue" : 0,
		"maxValue" : 4294967295,
		"defaultValue" : 20250910,
		"name" : "g_config.airport_limit_cfg.cfg_limit_data"

GEOZONES DISABLED
		"index" : 4,
		"typeID" : 0,
		"size" : 1,
		"attribute" : 51,
		"minValue" : 0,
		"maxValue" : 1,
		"defaultValue" : 0,
		"name" : "g_config.flying_limit.viechle_license_limit_enable"
{
		"index" : 3,
		"typeID" : 0,
		"size" : 1,
		"attribute" : 50,
		"minValue" : 0,
		"maxValue" : 1,
		"defaultValue" : 0,
		"name" : "g_config.flying_limit.driver_license_limit_enable"
{
		"index" : 1,
		"typeID" : 0,
		"size" : 1,
		"attribute" : 57,
		"minValue" : 0,
		"maxValue" : 255,
		"defaultValue" : 1,
		"name" : "g_config.airport_limit_cfg.cfg_dis
		
		"index" : 31,
		"typeID" : 2,
		"size" : 4,
		"attribute" : 45,
		"minValue" : 0,
		"maxValue" : 65535,
		"defaultValue" : 1,
		"name" : "g_config.airport_limit_cfg.cfg_search_radius"
*********************************************************************************************************		
		ENABLE MOTORS TO BE RESTARTED WHEN AIRCRAFT INVERTED
		"index" : 7,
		"typeID" : 0,
		"size" : 1,
		"attribute" : 39,
		"minValue" : 0,
		"maxValue" : 1,
		"defaultValue" : 1,
		"name" : "g_cfg_debug.motor.no_start_motor_check"


		"index" : 980,
		"typeID" : 0,
		"size" : 1,
		"attribute" : 46,
		"minValue" : 0,
		"maxValue" : 1,
		"defaultValue" : 1,
		"name" : "g_config.fdi_open.close_auto_stop_motor_check"
*********************************************************************************************************	

{Widened MIN/MAX Yaw speed range for P-GPS with OA sensors ON
		"index" : 152,
		"typeID" : 8,
		"size" : 4,
		"attribute" : 41,
		"minValue" : 1.000000,
		"maxValue" : 200.000000,
		"defaultValue" : 70.000000,
		"name" : "g_config.avoid_cfg.avoid_tors_rate_range"

{Widened MIN/MAX Yaw speed range for P-GPS with OA sensors OFF
		"index" : 730,
		"typeID" : 8,
		"size" : 4,
		"attribute" : 41,
		"minValue" : 1.000000,
		"maxValue" : 300.000000,
		"defaultValue" : 90.000000,
		"name" : "g_config.mode_normal_cfg.tors_gyro_range"

{Widened MIN/MAX Yaw speed range for beginner mode
		"index" : 719,
		"typeID" : 8,
		"size" : 4,
		"attribute" : 41,
		"minValue" : 1.000000,
		"maxValue" : 300.000000,
		"defaultValue" : 70.000000,
		"name" : "g_config.mode_gentle_cfg.tors_gyro_range"
	},
{Widened MIN/MAX Yaw speed range for sport mode
		"index" : 741,
		"typeID" : 8,
		"size" : 4,
		"attribute" : 40,
		"minValue" : 1.000000,
		"maxValue" : 300.000000,
		"defaultValue" : 150.000000,
		"name" : "g_config.mode_sport_cfg.tors_gyro_range"
	},
{Widened MIN/MAX Yaw speed range for prop cage mode
		"index" : 752,
		"typeID" : 8,
		"size" : 4,
		"attribute" : 40,
		"minValue" : 1.000000,
		"maxValue" : 250.000000,
		"defaultValue" : 90.000000,
		"name" : "g_config.prop_cover_cfg.tors_gyro_range"
		
{Widened MIN/MAX Yaw speed range for Cinematic mode
		"index" : 760,
		"typeID" : 8,
		"size" : 4,
		"attribute" : 14,
		"minValue" : 1.000000,
		"maxValue" : 250.000000,
		"defaultValue" : 50.000000,
		"name" : "CM_tors_range"
	},
{Widened MIN/MAX Yaw speed range for tripod mode
		"index" : 774,
		"typeID" : 8,
		"size" : 4,
		"attribute" : 41,
		"minValue" : 1.000000,
		"maxValue" : 300.000000,
		"defaultValue" : 15.000000,
		"name" : "g_config.mode_tripod_cfg.tors_gyro_range"
		
{Widened MIN/MAX Yaw speed range for manual mode
		"index" : 783,
		"typeID" : 8,
		"size" : 4,
		"attribute" : 41,
		"minValue" : 1.000000,
		"maxValue" : 500.000000,
		"defaultValue" : 150.000000,
		"name" : "g_config.mode_manual_cfg.tors_gyro_range"
	},
{Widened MIN/MAX Yaw speed range for waypoint mode 
		"index" : 807,
		"typeID" : 8,
		"size" : 4,
		"attribute" : 40,
		"minValue" : 1.000000,
		"maxValue" : 300.000000,
		"defaultValue" : 90.000000,
		"name" : "g_config.waypoint_cfg.max_auto_yaw_rate"
		{
*********************************************************************************************************	
	},
{Widened MIN/MAX vertical speed range in tripod mode 
		"index" : 775,
		"typeID" : 8,
		"size" : 4,
		"attribute" : 37,
		"minValue" : 0.500000,
		"maxValue" : 10.000000,
		"defaultValue" : 1.000000,
		"name" : "g_config.mode_tripod_cfg.vert_vel_up"
	},
		"index" : 776,
		"typeID" : 8,
		"size" : 4,
		"attribute" : 39,
		"minValue" : -10.000000,
		"maxValue" : -0.500000,
		"defaultValue" : -1.000000,
		"name" : "g_config.mode_tripod_cfg.vert_vel_down"
	},

