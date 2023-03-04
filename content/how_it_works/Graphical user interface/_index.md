+++
title = "Graphical user interface"
date = 2023-02-25T07:26:45+01:00
weight = 1
chapter = false
+++

### Menu structure


You can find a pdf version of the document describing the user interface here (in french only for now).
{{%attachments style="orange" /%}}

## START:
![](start_and_acquisition.jpg)
Start acquisition sequence. Pressing the cursor during acquisition cancels the current sequence.
## Infos:
![](infos_and_firmware.jpg)
Display firmware version.
## Settings:
![image](settings.JPG)
Adjust settings related to exposure time, camera triggering, motor steps, illumination duration, etc.
### Motor:
![image](motor.JPG)
#### Stab. delay:
![image](stabilisation_delay.JPG)
Delay for stabilizing the fork. Wait time before the first shot after the fork reaches its position. Increasing this delay avoids potential blur effects on the first shot induced by system vibration at the end of movement. Recommended value minimum 50ms.
#### Motor speed:
![image](motor_speed.JPG)
Maximum motor movement speed in steps/s.
#### Calibrate:
![](calibrate.JPG)
![](calibrate_now.JPG)
"Calibrate now" starts the motor calibration process, searching for the end-of-travel contact to reset the motor step counter.
### Acquisition:
![image](acquisition.JPG)
The fork position is given on a scale from **0 to 1**.
![image](02_27_23_09_12_16-r2.jpg)
**Position 0** represents the **minimum position** determined by calibration (end-of-travel sensor position), and **position 1 represents the maximum** motor position.
#### Steps count:
![image](steps_count.JPG)
Number of polar positions for measurement.
#### Min position:
![](min_position.JPG)
![](min_polar_position.JPG)
First polar position of the fork.
#### Max position:
![](max_position.JPG)
![](max_polar_position.JPG)
Last polar position of the fork.
### Photo Trigger:
![image](photo_trigger.JPG)
#### Shutter type:
![image](shutter_type.JPG)
Trigger type, by dry contact with internal relay (relay) or by infrared signal (IR).
### IR Signal:
![image](ir_signal.JPG)
#### Predefined:
![](ir_predefined.JPG)
![](ir_mode_nikon.JPG)
Choose the trigger signal from commonly used camera brands. Choose "custom" to use your own signal.
#### Record IR:
![image](record_ir.JPG)
Record your own signal from the camera's original remote (feature not implemented yet, require to add an IR sensor to Hasor arduino shield)
### Shutter Duration:
![image](shutter_duration.JPG)
Duration of dry contact for camera triggering via relay (sync cable). Adjust according to the camera.
### Snaps delay:
![image](snaps_delay.JPG)
Minimum time between two shots.
## Leds:
![image](leds.JPG)
Section for adjusting LEDs parameters.
### Modules count:
![image](module_count_setting.JPG)
Number of LED modules. 6 by default.
### Leds by module:
![image](leds_by_module.JPG)
Number of LEDs per module. Set to 3 in the case of RGB LED modules on LED modules.
### Tune intensities:

{{row}}
{{column}}![](led_tuning_led_id.JPG) {{/column}}
{{column}}![](led_tuning_setting.JPG) else{{/column}}
{{column}}![](led_tuning_exit.JPG) else{{/column}}
{{/row}}

Adjust LED intensity by module. Turn the knob to select led number 0 to MAX_LED. Pushing the knob let you enter into setting mode. Turn the knob to set new intensity (in percent of the max intensity defined into related section). Push again to validate. To exit led tuning menu, rotate knob until showing "Exit" and push to validate. 
### LedOn duration:
![](ledon_duration.JPG)
![](led_on_delay.JPG)
Duration of LED triggering, adjust to be at least equal to the camera's exposure time.
## Tests:
![image](tests.JPG)
Section for testing LEDs, camera triggering, or motor movement.
### Motor:
![](motor2.JPG)
![](motor_test.JPG)
Turn the cursor to move the fork and check the status of the end-of-travel sensor(s). Click to return to the previous menu.
### Shutter:
![](shutter.JPG)
![](trigger_now.JPG)
**"Trigger now"** triggers the camera with the settings defined in "settings" section.
### Leds:
![image](launch_test.JPG)
**"Launch test"** triggers a sequential lighting **test of all LEDs**.
## Save:
![](save_parameters.JPG)
![](parameters_saved.JPG)
Save the settings previously defined by the user (min/max position, steps count, etc.) in one of the available memory slots. Click on the **configuration name** to save or **"Cancel"** to return to the previous menu.
## Load:
![](load_parameters.JPG)
![](parameters_loaded.JPG)
Load the settings previously **saved by the user**. Click on the **configuration name** to load or **"Cancel"** to return to the previous menu.