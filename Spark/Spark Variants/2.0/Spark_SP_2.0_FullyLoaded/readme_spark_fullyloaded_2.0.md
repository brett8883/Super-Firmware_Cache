====CUSTOM DJI SPARK FLIGHT CONTROLLER MODULE====

Compiled by Brett8883 using Matoupi's FC_Patcher via Brett8883's Super-Patcher

**MUST be installed via Brett8883’s Super Patcher https://github.com/brett8883/DJI_Super-Patcher **

===
FLIGHT CONTROLLER version #

Height limits disabled 

NFZ limits disabled 

GeoZone limits disabled 

Yaw speed min/max paramter ranges extended 

Galileo GPS Satellites reception enabled

Motors will start if inverted (if CSC at altitude and AC inverts the motors will start to save it)

Possible smart battery warning levels expanded 

Rear LED light disabled in flight




===

Notes From the Author:
• Smart Battery Mod Super Patcher 2.0 Custom Flight Controller for Spark

• Smart battery configured to neve force auto-land due to low battery except at the emergency battery voltage at 3.0v per cell

• Rear LED lights disabled in flight
  - Lights still turn on during start up 
===

***Firmware Compatibility:***

To use this Custom firmware, your DJI Spark MUST BE ON STOCK FW v01.00.0900

===

Know what you are doing before you use this.
********************************************************************************************

Change Log


HEIGHT LIMIT DISABLED

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

		"minValue" : 0,
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

Widened MIN/MAX Yaw speed range for P-GPS with OA sensors OFF

		"minValue" : 1.000000,
		"maxValue" : 300.000000,
		"defaultValue" : 90.000000,
		"name" : "g_config.mode_normal_cfg.tors_gyro_range"

Widened MIN/MAX Yaw speed range for beginner mode

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

		"minValue" : 1.000000,
		"maxValue" : 250.000000,
		"defaultValue" : 50.000000,
		"name" : "CM_tors_range"

Widened MIN/MAX Yaw speed range for tripod mode

		"minValue" : 1.000000,
		"maxValue" : 300.000000,
		"defaultValue" : 15.000000,
		"name" : "g_config.mode_tripod_cfg.tors_gyro_range"
		
Widened MIN/MAX Yaw speed range for manual mode

		"minValue" : 1.000000,
		"maxValue" : 500.000000,
		"defaultValue" : 150.000000,
		"name" : "g_config.mode_manual_cfg.tors_gyro_range"

Widened MIN/MAX Yaw speed range for waypoint mode 

		"minValue" : 1.000000,
		"maxValue" : 300.000000,
		"defaultValue" : 90.000000,
		"name" : "g_config.waypoint_cfg.max_auto_yaw_rate"
		
*********************************************************************************************************	
# Variant Changes

Disabled forced autoland at critical battery warning 

		"minValue" : 0,
		"maxValue" : 2,
		"defaultValue" : 0,
		"name" : "bat_level_2_action"

Disabled battery warning levels (can be reenabled in Assistant 1.1.2)

		"minValue" : 0,
		"maxValue" : 100,
		"defaultValue" : 0,
		"name" : "dji_bat_level_1"
		
		"minValue" : 0,
		"maxValue" : 100,
		"defaultValue" : 0,
		"name" : "dji_bat_level_2
		
Disabled forced auto-landing at only enough battery to land level

		"minValue" : 0,
		"maxValue" : 1,
		"defaultValue" : 0,
		"name" : "g_config.bat_config.enable_smart_bat_landing_portect"

Changed calculations of only enough battery to return to the home point to make it more accurate

		"minValue" : 0,
		"maxValue" : 100,
		"defaultValue" : 5,
		"name" : "smart_bat_basic_cap"
		
Disabled smart rth and smart landing by default(can be adjusted in DJI Go or Assistant 2 1.1.2 in debug mode

		"minValue" : 0,
		"maxValue" : 100,
		"defaultValue" : 0,
		"name" : "g_config.bat_config.level1_smart_battert_gohome"
	
		"minValue" : 0,
		"maxValue" : 100,
		"defaultValue" : 0,
		"name" : "g_config.bat_config.level2_smart_battert_land"

***
Disable rear LED lights while in flight

		"minValue" : 0,
		"maxValue" : 1,
		"defaultValue" : 0,
		"name" : "g_cfg_debug.force_flash_led"


