<p align="center">
  <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Kingia%20Castle.png" width="250"/>
</p>
<h1 align="center">Kingia Castle Smart Home Configuration</h1>
<hr *** </hr>
<p align="center">Home Assistant Configuration &amp; Documentation for my Smart House.</p>
<p align="center">
  I live in <img src="https://github.com/oxguy3/flags/blob/master/mini/au.png"/>, and therefor my links are for where I purchased from. There may be better (and most likely cheaper) sites in your local regions.
</p>
<hr --- </hr>

### Home Assistant Hardware Topology
<p align="center">
  <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/HA%20Topo.png"/>
</p>
<hr --- </hr>

<h3 align="left">Home Assistant Hardware</h3> 
<img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Rasp%20Pi%20Logo.png" width="200"/> 
<p align="left">There is nothing special regarding the hardware used when I start to notice available hardware resources becoming exhausted I will look to move to another platform. 
<hr --- </hr>


| [Raspberry Pi 3 Model B+](https://core-electronics.com.au/raspberry-pi-3-model-b-plus.html) | [Raspberry Pi 3 Model B+ Enclosure](https://core-electronics.com.au/raspberry-pi-3-case-enclosure.html) | [SandDisk Ultra 32GB Micro SD Card](https://www.officeworks.com.au/shop/officeworks/p/sandisk-ultra-32gb-micro-sdhc-memory-card-sdsq32gb) | [Raspberry Pi 3+ Power Supply](https://core-electronics.com.au/raspberry-pi-3-power-supply.html) |
| --- | --- | --- | --- |
| <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/raspberry-pi-3-model-b_-plus.png" width="250"/> | <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Rasp%20Pi%20Case.png" width="250"/> | <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Micro%20SD%20Card.png" width="200"/> | <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Rasp%20Pi%20PSU.jpg" width="250"/> |

<h3 align="left">Home Assistant Software</h3>
<img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/HA%20logo%202%20.png" width="200"/>
<h4 align="left">Hassio:</h4>
<p align="left">As I am still new and always learning to Home Assistant, I decided to install HASSIO. I have been using HASSIO for since December 2017 for anyone new to HA I recommend this type of installation and once you are more comfortable with it I would look to move onto some of the other methods of installation.</p>
<h4 align="left">MQTT Broker:</h4>
One of the first things I needed to do once I got HA up and running was to setup a MQTT Broker, I decided to use [Owntracks]: https://www.home-assistant.io/components/device_tracker.owntracks as I found this really helpful guide from <[BRUH](https://www.youtube.com/watch?v=VaWdvVVYU3A)/> and was up and running in 15mins. The main problem I had with this method was using a cloud based service to control my mqtt based light switches, using Owntracks for Device Tracking was also not what was required for Automations based of presence. I decided to install Mosquitto Broker from the Hass.io Add-On Store. Doing this means I can host the MQTT Broker locally therefor having control of who can access my devices and data.
[Owntracks](https://www.home-assistant.io/components/device_tracker.owntracks)
<hr --- </hr>

| [Hass.io](https://www.home-assistant.io/hassio/installation/) | [Mosquitto MQTT Broker](https://www.home-assistant.io/addons/mosquitto/) | [AppDaemon - HADashboard](https://www.home-assistant.io/docs/ecosystem/appdaemon/) | [Node-RED](https://github.com/notoriousbdg/hassio-addons/tree/master/node-red) |
| --- | --- | --- | --- |
| <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/HA%20logo.png" width="250"/> | <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Mosquitto%20MQTT%20Logo.png" width="250"/> | <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/appdaemon.PNG" width="250"/> | <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Node-RED%20Logo.png" width="250"/> |


<hr ---</hr>
