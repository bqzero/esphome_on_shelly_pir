# esphome_on_shelly_pir
As I faced issues setting up my shellies to work with none momentary PIR sensors I investigated for solutions.
Turns out it is impossible to achieve the desired result with a shelly 1 specially the Gen1 which has no scripts option.

Therefore I have created a ESPHome alternative config that works like a charm. To use it you will have to do the following

## Adjust the shelly.yaml
Change the device name and description to your liking
```
device_name: shelly
device_description: "shelly"
```
either provide the secrets required or replace them with your values
```
!secret api_key
!secret ota_password
!secret wifi_ssid
!secret wifi_password
!secret ap_wifi_password
```
## Flash the configuration
Choose your way on how to flash the configuration, I myself prefer the option to flash over a USB to TTL, but you are of course
free on how to flash it. Other ways can be found online.

Flashing using adapter (as example)
https://www.youtube.com/watch?v=0hQdxa2wQJE

