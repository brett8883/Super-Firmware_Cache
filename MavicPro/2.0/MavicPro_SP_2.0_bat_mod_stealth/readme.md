# 2.0 UPDATES

Disabled forced autoland at critical battery warning

		"minValue" : 0,
		"maxValue" : 2,
		"defaultValue" : 0,
		"name" : "bat_level_2_action"

Lowered battery warning levels to 1% (can be adjusted in DJI Go 4 or in Assistant 1.1.2 note: Setting these level to zero disables the warning levels altogether and makes it so they can't be adjusted in DJI Go 4)

		"minValue" : 0,
		"maxValue" : 100,
		"defaultValue" : 1,
		"name" : "dji_bat_level_1"
		
		"minValue" : 0,
		"maxValue" : 100,
		"defaultValue" : 1,
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
