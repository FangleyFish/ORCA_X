***Schematic Notes***



**Controller:**



Key switch in between power source and Pico.



Covered toggle switch on input pin to be used for software safety switch



Two momentary push buttons wired in series on an input pin to be used for countdown activation.



Big red 2 position push/pull lockdown button, when pressed, breaks circuit of covered toggle switch to pin, also breaks circuit of double push buttons to pin, is also wired to an input pin to initiate base sation safe mode (which does some more breaking of circuits on the base station side)



An OLED display is wired on I2C bus for status HUD.



Two 8-segment number displays show countdown timer numericals.



LED light for continuity indication for motor igniter. (sent from base station)



Flashing LED light for 'ready to launch' indication (sent from base station)



**Base Station:**


Dewalt Battery ✔

Dewalt Battery Connector ✔ Use screw terminals
	- What is the gauge of the wires?

Engine Ignition 
	- What have you used for ignition before?

Shutdown switch 
	- No problem 

UVLO in hardware 
	- What Voltage are the batteries we are using? 
	- What is the lowest acceptable Voltage before we should cut off?
	
	- Send signal to Pico for safe shutdown
	- Check for Pico to signal safe shutdown completed
	- Cut power regardless if Voltage is too low
	- UVLO indicator LED and indicator buzzer?

Power cut circuit 
	
Power Indicator LED

Flashing Ready Indicator LED - What are the ready conditions?
	- Shutdown switch = not in shutdown state
	- Signal from Lauch Controller rx by the Pi

Bright Orange Flashing Caution Countdown LED - and buzzer?



