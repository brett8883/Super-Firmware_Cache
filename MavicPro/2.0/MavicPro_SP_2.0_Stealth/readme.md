Flight Controller#03.02.44.12

Rear LED to remain off in flight (hard-coded value cannot be changed by user. to re-enable requires flash to stock firmware

		"minValue" : 0,
		"maxValue" : 1,
		"defaultValue" : 0,
		"name" : "g_cfg_debug.force_flash_led"

Extended configuable range for DJI battery levels (these are the absolute battery levels and different from smart battery levels) default values remain factory default
		
		"minValue" : 0,
		"maxValue" : 100,
		"defaultValue" : 30,
		"name" : "dji_bat_level_1"

		"minValue" : 0,
		"maxValue" : 100,
		"defaultValue" : 10,
		"name" : "dji_bat_level_2"

