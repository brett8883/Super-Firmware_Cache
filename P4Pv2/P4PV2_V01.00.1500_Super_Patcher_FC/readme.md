# Super-Patcher Standard P4Pv22 V01.00.1500 FLIGHT CONTROLLER + + available smart battery mod + available sensitivity ranges 

Compiled by Brett8883 using Matoupi's FC_Patcher via Brett8883's Super-Patcher

**MUST be installed via Brett8883’s Super Patcher https://github.com/brett8883/DJI_Super-Patcher **

===
FLIGHT CONTROLLER version # 03.03.04.36

Height limits disabled 

NFZ limits disabled 

GeoZone limits disabled 

Yaw speed min/max paramter ranges extended (defaults remain factory default) 

Galileo GPS Satellites reception enabled

Widened DJI Smart Battery levels (defaults remain factory default)

Widened possible Sensitivity ranges (defaults remain factory default)


===

Notes From the Author:
• Standard Super-Patcher flight controller with some additional optional features. The DJI battery levels can be modified with Assistant 2 1.1.2 in debug mode allowing full control of the smart battery behavior and actions negating the need to switch to non-DJI Battery mode. This is available to be changed but by default these values are factory default. 

• NOTE: On P4Pv2 the unlimited height parameter does not fuction as expected so the actual hight limit has been increased to 9000m by default **effectively** granting unlimited height in practice. The user should not attempt to change the value for height limit from within the app as the DJI GO 4 app will not accept a new height limit value above 500m however it will allow a higher value if the value is entered in Assistant 2 1.1.2 in debug mode, or in this case, if the value above 500m is hard-coded as the default value. However, changing this value in the app risks relocking the height limit due to the app not allowing a new value above 500m.  

• Sensitivity ranges can be changed is assistant 2 1.1.2 to fine tune the response to stick input. Think of sensitivity as how quickly the flight controller responds to a stick input with out changing the gain or PID settings. Changes may have to be large to give the pilot a noticable change when testing but getting use to one sensitivity setting and then changing to another will be noticable in regular flight. Values below 20 for sensitivity for any of the axies may have a larger effect then changes to sensitivity above 20. These values are factory default by default and requires Assistant 2 1.1.2 to change the sensitivity settings. Tilt-sensitivity is the same parameter as attitude sensitivity in the DJI Go4 app but the app may not save a value change that is less than 20 even though it may show this is possible. It is better to adjust these settings via Assistant 2 1.1.2 in debug mode  
===

***Firmware Compatibility:***

To use this Custom firmware, your DJI P4Pv2 MUST BE ON fully STOCK FW V01.00.1500

===

Know what you are doing before you use this.
********************************************************************************************

Full Change Log for Super-Patcher Standard Spark DJI Super-Patcher Custom Flight Controller

*this list includes ALL paramters that were changed even hardcoded values (galileo not config with parameters)

HEIGHT LIMIT DISABLED

		"minValue" : 0,
		"maxValue" : 1,
		"defaultValue" : 0,
		"name" : "limit_height"

		"minValue" : 1,
		"maxValue" : 2,
		"defaultValue" : 2,
		"name" : "g_config.flying_limit.height_limit_enabled",
		"alias" : "g_config.advanced_function.height_limit_enabled",
		"modify" : true

		"minValue" : 0.000000,
		"maxValue" : 100000.000000,
		"defaultValue" : 10000.000000,
		"name" : "limit_height_abs_without_gps"
	

		"minValue" : 0.000000,
		"maxValue" : 100000.000000,
		"defaultValue" : 10000.000000,
		"name" : "limit_height_abs"
	
		"minValue" : 0.000000,
		"maxValue" : 100000.000000,
		"defaultValue" : 10000.000000,
		"name" : "limit_height_rel"

		"minValue" : 20,
		"maxValue" : 9000,
		"defaultValue" : 9000,
		"name" : "g_config.flying_limit.max_height"

Disable height limit during RTH

                "minValue" : 0,
		"maxValue" : 1,
		"defaultValue" : 1,
		"name" : "avoid_ascending_height_limit_disable",
		"alias" : "g_config.go_home.avoid_ascending_height_limit_disable"

	
NFZ DISABLE

		"minValue" : 0,
		"maxValue" : 1,
		"defaultValue" : 1,
		"name" : "cfg_disable_airport_fly_limit"
		

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
		
*********************************************************************************************************		
		ENABLE MOTORS TO BE RESTARTED WHEN AIRCRAFT INVERTED
		
		"minValue" : 0,
		"maxValue" : 1,
		"defaultValue" : 1,
		"name" : "motor_no_start_motor_check",
		"modify" : true

		"minValue" : 0,
		"maxValue" : 1,
		"defaultValue" : 1,
		"name" : "g_config.fdi_open.close_auto_stop_motor_check"
*********************************************************************************************************	

Widened MIN/MAX Yaw speed range for P-GPS with OA sensors ON
	
		"minValue" : 1.000000,
		"maxValue" : 150.000000,
		"defaultValue" : 70.000000,
		"name" : "avoid_cfg_tors_rate_range",
		"alias" : "g_config.avoid_cfg.avoid_tors_rate_range"
	

Widened MIN/MAX Yaw speed range for P-GPS with OA sensors OFF

		"minValue" : 1.000000,
		"maxValue" : 250.000000,
		"defaultValue" : 150.000000,
		"name" : "g_config.mode_normal_cfg.tors_gyro_range"


Widened MIN/MAX Yaw speed range for sport mode

		"minValue" : 1.000000,
		"maxValue" : 300.000000,
		"defaultValue" : 250.000000,
		"name" : "g_config.mode_sport_cfg.tors_gyro_range"
		
Widened MIN/MAX Yaw speed range for Cinematic mode
	
		"minValue" : 1.000000,
		"maxValue" : 250.000000,
		"defaultValue" : 50.000000,
		"name" : "CM_tors_range"
	
Widened MIN/MAX Yaw speed range for tripod mode

		"minValue" : 1.000000,
		"maxValue" : 150.000000,
		"defaultValue" : 60.000000,
		"name" : "g_config.mode_tripod_cfg.tors_gyro_range"
		
***************************************************	

Widened MIN/MAX vertical speed range in tripod mode 
		
		"minValue" : 0.500000,
		"maxValue" : 10.000000,
		"defaultValue" : 1.500000,
		"name" : "g_config.mode_tripod_cfg.vert_vel_up"
	
		"minValue" : -10.000000,
		"maxValue" : -0.500000,
		"defaultValue" : -1.500000,
		"name" : "g_config.mode_tripod_cfg.vert_vel_down"

***************************************************

Widened DJI Smart Battery levels (defaults remain factory default) 

		"minValue" : 0,
		"maxValue" : 100,
		"defaultValue" : 30,
		"name" : "dji_bat_level_1",
		"alias" : "g_config.voltage2.level_1_voltage"

		"minValue" : 0,
		"maxValue" : 100,
		"defaultValue" : 10,
		"name" : "dji_bat_level_2",
		"alias" : "g_config.voltage2.level_2_voltage"

***************************************************

Widened possible Sensitivity ranges (defaults remain factory default)

		"minValue" : 1,
		"maxValue" : 100,
		"defaultValue" : 50,
		"name" : "tilt_sensitive_gain",
		"alias" : "g_config.control.rc_tilt_sensitivity"

		"minValue" : 1,
		"maxValue" : 100,
		"defaultValue" : 50,
		"name" : "yaw_sensitive_gain"

		"minValue" : 1,
		"maxValue" : 100,
		"defaultValue" : 100,
		"name" : "rc_throttle_sensitivity"