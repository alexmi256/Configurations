## Eryon Thinker S V2
Based off of the Thinker SE config. 
To be honest I'm not sure what the different is between the Thinker S V2 vs. the SE 
I know the S V2 has TMC2208 drivers which I was surprised to see were not enabled on the THINKER config.

 - BLTouch probe
 - TMC2208 (standalone) stepper drivers
 - PIDTEMPBED enabled
 - I find that if I ever try to fully heat up the hotend while it's already +150*C from a previous print or setup I get heating errors so:
	 - Increased THERMAL_PROTECTION_PERIOD 40 -> 60
	 - Increased #define WATCH_TEMP_PERIOD  20 -> 40
