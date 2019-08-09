# Spark No Inverted Motor Restart

Compiled by Brett8883 using Matoupi's FC_Patcher via Brett8883's Super-Patcher

**MUST be installed via Brett8883’s Super Patcher https://github.com/brett8883/DJI_Super-Patcher **

===
FLIGHT CONTROLLER version # **03.02.43.08**

Height limits disabled 

NFZ limits disabled 

GeoZone limits disabled 

Yaw speed min/max paramter ranges extended 

Galileo GPS Satellites reception enabled

===

**Notes From the Author:**

• Same as the Standard Super-Patcher Super-Patcher flight controller but does not have the parameters to restart motors when inverted. This allows the pilot to cut the motors after a hand catch by tipping it over past 90 degrees. No other changes

**Firmware Compatibility:**

To use this Custom firmware, your DJI Spark MUST BE ON STOCK FW **v01.00.0900**

===

Know what you are doing before you use this.
********************************************************************************************

Full Change Log

*this list includes ALL paramters that were changed even hardcoded values (Galileo not config with parameters)

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
		"maxValue" : 255,
		"defaultValue" : 1,
		"name" : "g_config.airport_limit_cfg.cfg_disable_airport_fly_limit"
		
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
**************************************

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

Widened MIN/MAX vertical speed range in tripod mode
 
		"minValue" : 0.500000,
		"maxValue" : 10.000000,
		"defaultValue" : 1.000000,
		"name" : "g_config.mode_tripod_cfg.vert_vel_up"
		
		"minValue" : -10.000000,
		"maxValue" : -0.500000,
		"defaultValue" : -1.000000,
		"name" : "g_config.mode_tripod_cfg.vert_vel_down"


