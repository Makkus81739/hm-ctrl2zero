# A Python program for controlling Hoymiles inverters (HM-Series)
This program is used to control a Hoymiles inverter in a way that it minimizes the amount of solar generated power going to the public grid (zero-export). In combination with a battery it support a maximized self-usage of the solar power.

It runs on a Raspberry Pi with a nRF24L01+ board connected and using either a Tasmota device or a Shelly 3EM to fetch data from the power meter.

The functions controling the inverter through the nRF24L01+ module are based on the great works of https://github.com/Knedox/hoymiles_control.
The core functions implementing the zero-control capability were developed by https://github.com/eenemeenemuu/hoymiles_zero_export.

## Basic requirements
Additionally to what [eenemeenemuu](https://github.com/eenemeenemuu/hoymiles_zero_export/commits?author=eenemeenemuu) describes on his Github page this code was also successfully tested with:
- Hoymiles HM-1200 inverter
- Raspberry Pi 2B
- Tasmota 12.4.0 running on a Wemos D1 with a Hitchi IR read head connected

Make sure that all mentioned device are installed properly and you can reach them over your home network.
