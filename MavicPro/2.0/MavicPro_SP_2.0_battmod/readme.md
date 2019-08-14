MavicPro SP 2.0 Standard
FC#: 03.02.44.21

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
