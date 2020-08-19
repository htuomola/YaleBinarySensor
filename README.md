# YaleBinarySensor
Yale Smart Alarms Binary Door Sensors for Homeassistant

Add to config/custom_components/yalebinarysensor

Need to add the following to your configuration.yaml

~~~text
binary_sensor:
  - platform: yalebinary
    username: <YALE USERNAME>
    password: <YALE PASSWORD>
~~~
  
it will add binary sensors for all your door/window contacts

binary_sensor(New).py is a new way of dealing with the data and pulling more information out. To make this work, rename it to binary_sensor.py replacing the old one in config/custom_components/yalebinarysensor

e.g. binary_sensor.back_door

All credit to the homeassistant devs and the following without which it would not be possible
https://github.com/domwillcode/yale-smart-alarm-client
