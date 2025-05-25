# TinyPowerController
ATTINY85 based tunable LiPo charger with load switch, button and multiple UX footprint options

	Designed: 2019 02 16
	Cleaned up: 2025 05 24

	Summary:
		1 sqaure inch power controller for low power devices.
		LiPo charger with USB micro input.
		ATTINY85 for measuring battery voltage, temperature and button timing.
		Load switch for turning off downstream device.

	Charging Current:
		Pchrg is header for adjusting charging current.
		0ohm: 500mA
		4.5kohm: 200mA
		open: 50mA
		If R1 is removed and Pchrg = 64.8kohm: 15mA
		See schematic for equations.
		
	Battery voltage measurement:
		Interally connect Vref to ADC input and VCC to ADC ref.
		Sounds strange but this 'pinless' Vcc measurement does work with ATTINY85!
		
	Coin Cell Holder:
		LIR2032 holder (straight, T/H), pins fit into H1 and H3.
		Place positive pin thru H3 so it can connect to BAT+
		
	Mounting Options:
		Multi footprints were used for USB and button.
		USB: top or bottom, straight or R/A.
		Button, top: straight or R/A.
		Button, bottom: R/A
		
