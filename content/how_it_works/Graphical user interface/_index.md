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
![image](start.jpg)
Start acquisition sequence. Pressing the cursor during acquisition cancels the current sequence.
## Infos:
![image](infos.jpg)
Display firmware version.
## Settings:
![image](settings.jpg)
Adjust settings related to exposure time, camera triggering, motor steps, illumination duration, etc.
### Motor:
![image](motor.jpg)
#### Stab. delay:
![image](stabilisation_delay.jpg)
Delay for stabilizing the fork. Wait time before the first shot after the fork reaches its position. Increasing this delay avoids potential blur effects on the first shot induced by system vibration at the end of movement. Recommended value: 50ms.
#### Motor speed:
![image](motor_speed.jpg)
Maximum motor movement speed. Recommended value: XX steps/s.
#### Calibrate:
![image](calibrate.jpg)
"Calibrate now" starts the motor calibration process, searching for the end-of-travel contact to reset the motor step counter.
### Acquisition:
![image](acquisition.jpg)
The fork position is given on a scale from **0 to 1**.
![image](02_27_23_09_12_16-r2.jpg)
**Position 0** represents the **minimum position** determined by calibration (end-of-travel sensor position), and **position 1 represents the maximum** motor position.
#### Steps count:
![image](steps_count.jpg)
Number of polar positions for measurement.
#### Min position:
![image](min_polar_position.jpg)
First polar position of the fork.
#### Max position:
![image](max_polar_position.jpg)
Last polar position of the fork.
### Photo Trigger:
![image](photo_trigger.jpg)
#### Shutter type:
![image](shutter_type.jpg)
Trigger type, by dry contact with internal relay (relay) or by infrared signal (IR).
### IR Signal:
![image](ir_signal.jpg)
#### Predefined:
![image](ir_predefined.jpg)
Choose the trigger signal from commonly used camera brands. Choose "custom" to use your own signal.
#### Record IR:
![image](record_ir.jpg)
Record your own signal from the camera's original remote.
### Shutter Duration:
![image](shutter_duration.jpg)
Duration of dry contact for camera triggering via relay (sync cable). Adjust according to the camera.
### Snaps delay:
![image](snaps_delay.jpg)
Minimum time between two shots.
## Leds:
![image](leds.jpg)
Section for adjusting LEDs parameters.
### Modules count:
![image](module_count.jpg)
Number of LED modules. 6 by default.
### Leds by module:
![image](leds_by_module.jpg)
Number of LEDs per module. Set to 3 in the case of RGB LED modules on LED modules.
### Tune intensities:
![image](tune_intensity.jpg)
Adjust LED intensity by module. TODO.
### LedOn duration:
![image](ledon_duration.jpg)
Duration of LED triggering, adjust to be at least equal to the camera's exposure time.
## Tests:
![image](tests.jpg)
Section for testing LEDs, camera triggering, or motor movement.
### Motor:
![image](motor.jpg)
Turn the cursor to move the fork and check the status of the end-of-travel sensor(s). Click to return to the previous menu.
### Shutter:
![image](shutter.jpg)
**"Trigger now"** triggers the camera with the settings defined in "settings" section.
### Leds:
![image](leds2.jpg)
**"Launch test"** triggers a sequential lighting **test of all LEDs**.
## Save:
![image](save_parameters.jpg)
Save the settings previously defined by the user (min/max position, steps count, etc.) in one of the available memory slots. Click on the **configuration name** to save or **"Cancel"** to return to the previous menu.
## Load:
![image](load_parameters.jpg)
Load the settings previously **saved by the user**. Click on the **configuration name** to load or **"Cancel"** to return to the previous menu.