Heated blanket automation
=========================

Home Assistant scripts to control a switch using PWM, based on a duty cycle percentage. This allows you to set your heated blanket to 100% and have it warm up before bedtime (or maybe in the morning), while not overwarming during the night.

I haven't turned this into a blueprint yet, so please create:

 - An input_select for the heated blanket, with options Warmup, Sustain and Idle.
 - A timer to run the PWM. Intervals are provided by the script so don't worry about settings.
 - Optionally, an input_number from 0 to 100 for the default duty cycle.

Then create the automations, pointing at your heated blanket switch. You can either set the duty cycle for each automation, or point at the input_number.

You can then use a schedule or automation trigger to set the input_select to Warmup at bed time.
