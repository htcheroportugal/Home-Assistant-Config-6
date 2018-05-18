<p align="center">
  <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Kingia%20Castle.png" width="250"/>
</p>
<h1 align="center">Kingia Castle Smart Home Configuration</h1>
<hr *** </hr>
<p align="center">Home Assistant Configuration &amp; Documentation for my Smart House.</p>
<p align="center">
  I live in <img src="https://github.com/oxguy3/flags/blob/master/mini/au.png"/>, and therefor my links are for where I purchased from. There may be better (and most likely cheaper) sites in your local regions.</br>
<hr --- </hr> 

| [Home Assistant Screenshots](https://github.com/JamesMcCarthy79/Home-Assistant-Config/tree/master/HA%20Pics/HA%20Screenshots) |
| --- |
| [<img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/HA%20Screenshots/01.%20Home.png"/>](https://github.com/JamesMcCarthy79/Home-Assistant-Config/tree/master/HA%20Pics/HA%20Screenshots) |

| [HADashboard Screenshots](https://github.com/JamesMcCarthy79/Home-Assistant-Config/tree/master/HA%20Pics/HADashboard%20Screenshots) |
| --- |
| [<img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/HADashboard%20Screenshots/HADash%20-%20Downstairs%20Panel.png"/>](https://github.com/JamesMcCarthy79/Home-Assistant-Config/tree/master/HA%20Pics/HADashboard%20Screenshots) |
<hr --- </hr>

### Smart Home Hardware Topology
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
<p align="left">I have used Hassio with standard Add-On store packages which include Appdaemon for use with HaDashboard, Mosquitto Broker for MQTT Broker & Node-RED for more complex Automation flows.</p>
<hr --- </hr>

| [Hass.io](https://www.home-assistant.io/hassio/installation/) | [Mosquitto MQTT Broker](https://www.home-assistant.io/addons/mosquitto/) | [AppDaemon - HADashboard](https://www.home-assistant.io/docs/ecosystem/appdaemon/) | [Node-RED](https://github.com/notoriousbdg/hassio-addons/tree/master/node-red) |
| --- | --- | --- | --- |
| <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/HA%20logo.png" width="250"/> | <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Mosquitto%20MQTT%20Logo.png" width="250"/> | <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/appdaemon.PNG" width="250"/> | <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Node-RED%20Logo.png" width="250"/> |

<h4 align="left">Home Assistant:</h4>
<p align="left">As I am still new to Home Assistant (and always learning), I decided to install HASSIO. I have been using HASSIO since December 2017, for anyone new to HA I recommend this type of installation and once you are more comfortable with it I would then look to move onto some of the other methods of installation.</p>
<h4 align="left">MQTT Broker:</h4>
One of the first things I needed to do once I got HA up and running was to setup a MQTT Broker, I decided to use CloudMQTT(https://www.cloudmqtt.com/) as I found this helpful guide from BRUH(https://www.youtube.com/watch?v=VaWdvVVYU3A) and was up and running in 15mins. The main problem I had with this method was using a cloud-based service to control my MQTT based light switches. I decided to install Mosquitto Broker from the Hass.io Add-On Store. Doing this means I can host the MQTT Broker locally therefore having control of who can access my devices and data.
<h4 align="left">AppDaemon3 - HADashboard:</h4>
I have a bunch of wall mounted tablets (Android & IOS) as well as RPi with 7" touchscreens and whilst I like the standard HA UI there is way too much going on for my wife and guests who need to interact with the smart home system. In cometh HADashboard, it wraps up your basic controls (lights, cooling, heating, music etc) into nice looking widgets that make using the smart home controls a breeze for any non-tech person in the house (everyone but me). 
<h4 align="left">Node-RED:</h4>
After using HA for a few months, I began to really enjoy the sometimes-complicated methods of using automations, I also came to realise some of the limitations in its implementations. I found a good repo with an easy to follow installation guide by NotoriousBDG here (https://github.com/notoriousbdg/hassio-addons/tree/master/node-red) this handles any of my more complicated flows and conditioning required for my Automations.
<hr --- </hr>
<hr --- </hr>

<h3 align="left">Kingia Castle Network</h3>
<img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Network%20Topo.png"/>
<p align="left">My Internet is a 100/40Mb/s FTTN solution where the fibre is terminated about 50m up the road and travels down phones lines (VDSL2+) for the remainder I typically achieve speeds of 92/35Mb/s. The core of my network switching devices are made up of Mikrotik Cloud Router Series, whilst my wireless network is comprised of both Altai and UBNT devices. I use a VPN and isolate my Smart Home devices from my Personal and Guest access networks through VLAN's and client isolation is implemented on the guest network.</p>
<hr --- </hr>

| [Core Router](https://mikrotik.com/product/CCR1009-7G-1C-PC) | [Core Switch](https://mikrotik.com/product/CRS125-24G-1S-IN) | [Upstairs Switch](https://mikrotik.com/product/CRS106-1C-5S) | [Cabling]() |
| --- | --- | --- | --- |
| <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/CCR1009.jpg" width="250"/> | <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/CRS-125.jpg" width="350"/> | <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/CRS106.png" width="250"/> | <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Cabling.png" width="350" height="250"/> |

| [Altai A2c Dual-Band Access Point](https://www.powertec.com.au/altai-a2c-indoor-dual-band-2x2-802-11ac-ap-ceiling-mount) | [UBNT NanoBeam AC 5Ghz GEN2 19DBi](https://www.powertec.com.au/ubiquiti-nanobeam-ac-5ghz-gen2-19dbi-450mbps) | [UBNT NanoBeam AC 5Ghz GEN2 16DBi](https://www.powertec.com.au/ubiquiti-nanobeam-ac-5ghz-16dbi-450mbps) | [Network Management Tools]() |
| --- | --- | --- | --- |
| <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Altai-A2c.jpg" width="300"/> | <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Nano-19-AC.png" width="150"/> | <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Nano-19-AC.png" width="150"/> | <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Network%20Manage.png" width="350" height="250"/> |

<h4 align="left">Core Router:</h4>
<p align="left">My Core Router handles my PPPoE authentication, NAT and firewall rules. All my remote access is handled by a build it Cloud DNS service on the Mikrotik Router along with an extensive list of non-standard port forwards to gain access to every device I can remotely. I previously used the Mikrotik Device Tracker platform for online/offline status but found the response time too long so instead now use the Ping platform for device status monitoring.</p>
<h4 align="left">Core Switch:</h4>
<p align="left">My Core Switch is just a managed GBit Switch all my ethernet connected devices connect to this via Cat6 in wall Cabling into Cat6 Wall plates and all use Cat6 Patch Cables.</p>
<h4 align="left">Wireless Access:</h4>
<p align="left">I have 4 SSID one for each of admin access, family access, guest access & smart home device access. I used to run a Cambium cnPilot E400 which I was given by Cambium for testing in a "Conference Environment" it was meant to be able to handle 100 simultaneous YouTube streams well it started to fall over after about 35 connected clients (not streaming anything). Rather than filling the house with several APs I decided to go for the best in the business and am using a single Altai AP which is capable of handling 512 clients (currently have over 70 and still going strong). I only use 2.4G for access and have the 5G radio turned off as I use that spectrum for backhaul.</p>
<h4 align="left">Wireless PTMP Links:</h4>
<p align="left">I have a few impossible to cable areas of my 2-storey house (without running external ducting), between upstairs and downstairs and the outer wall of the downstairs area (where my media room is located). I have used a 19DBi UBNT NBE in AP mode connected directly to my Core Switch which links on 40Mhz channel to a unit in my media room and another upstairs which feed into a Mikrotik switch that connects any ethernet devices upstairs.</p>
<h4 align="left">Network Management:</h4>
<p align="left">I use Mikrotik for network configuration due to its highly configurable nature but it has a steep learning curve. I use these as I have been working with the product for over 12 years and am comfortable with it. I use winbox to access Mikrotik devices and prefer to do any configurations via the CLI, but the products do have a Web UI which is usable for most functions.</br> 

UBNT devices are configured by their Web UI and then managed by a CRM Point Device (overkill for 3 devices) they have been set and forget with only firmware upgrades performed if they address any security patches.</br> 

Altai AP is configured by its Web UI, these are commercial APs and are not designed with end users in mind. The UI is unpolished and hard to navigate if you don’t understand wireless and it is meant for wireless networking engineers. It is again highly configurable although there is nothing special here just 4 SSID (capable of up to 32) and VLAN tagging for each.</br>

The big bonus with Altai is their antenna design and ability to cover a great distance with a single AP and the amount of simultaneous connected clients it can handle. In my place so far, I have tried Mikrotik (coverage is poor due to low power and antenna design), UBNT (poor client handling and very susceptible to interference), Cambium (poor coverage and client handling was better than UBNT but not enough), Ruckus (great coverage poor client and roaming handover without controller)</p>
<hr --- </hr>
<hr --- </hr>

<h3 align="left">Voice Control & TTS</h3> 
<img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/alexa.png" width="150"/> 
<p align="left">The voice control war has only just hit Australian shores, I dipped my toes into the Alexa waters a few years back with the original Echo and it was a bit of a flop due to nothing being supported in Australia. Once I moved to HA and its Amazon cloud component I dusted off the Echo and now have voice control over a majority of my Smart Home.</p>
<hr --- </hr>

| [Amazon Echo](https://www.jbhifi.com.au/amazon/amazon-echo-plus-with-bonus-philips-hue-bulb-edison/574929/) | [Amazon Echo Dot](https://www.jbhifi.com.au/amazon/amazon-echo-dot-2nd-generation-black/574910/) | [Kodi TTS](https://www.home-assistant.io/components/notify.kodi/) | [Lannouncer](https://www.home-assistant.io/components/notify.lannouncer/) |
| --- | --- | --- | --- |
| <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Amazon%20-%20Echo.png" height="250"/> | <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Amazon%20-%20Dot.png" width="200"/> | <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Kodi%20Logo%202.png" width="200"/> | <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Google%20TTS.png" width="200"/> |

<h4 align="left">Voice Control:</h4>
<p align="left">I use a combination of Amazon Echo and Echo Dot's in conjunction with HA Cloud with its Alexa Integration to enable voice control over most functions in the house. My wife hates the voice control (she wants to be the only female voice of control in our house), but my young boys love it.</p>
* Light Control - LED Strips, Wall Switches and Bulb specific (Brightness, Colour, Warmth etc)</br>
* Climate Control - Control Upstairs/Downstairs Climate (temp up/down etc) turn ceiling fans on off (no speed control yet)</br>
* Media Control - Turn on/off Media Devices, player control of Kodi Media</br>
* Group Control - I can turn on/off all devices in a group e.g. "Alexa, turn off Downstairs" as we go to bed turns off all devices</br>
* Scene Selection - Enable predefined scenes with voice command</br>
* Automation Control - Perhaps the best part the ability to toggle Automations "Turn on Morning Cartoons", "Turn on &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;Entertaining mode"</br>
<h4 align="left">Announcements TTS</h4>
<p align="left">For TTS I use a combination of Kodi devices (I have one always on downstairs) and Android tablets with Lannouncer. I love the TTS and notifier component this is where you can start to give your Smart Home some personality as well as keep informed of events & reminders. I also use it for feedback after certain actions like confirmation of fan speed settings.</p>
* Notify of Presence - Unique messages played upon my wife and I arrival home</br>
* Notify of Tasks - Msg played when washer/dryer have finished their respective cycles, with 30min reminders until emptied</br>
* Reoccurring Events - Reminder msg to take out bins night before rubbish collection day, with alt msg for recycling week</br>
* Warning Events - Notify of Alarm Trigger, Arming, Outdoor Motion, Smoke/C02 Detection</br>
* Automation Notify - Notify on certain Automation runs like when sun is above horizon and lights are still on I turn them off &nbsp; &nbsp; and have TTS play a message "I guess I better turn the lights off or Tina will leave them on all day"
<hr --- </hr>
<hr --- </hr>

<h3 align="left">Gateways</h3> 

| <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Xiaomi%20Logo.png" width="150"/> | <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/SmartThings%20Logo.png" width="200"/> |
| --- | --- |

<p align="left">At the moment the majority of my sensors are Xiaomi, so I need to use their Gateway to integrate them with HA. I also have a Smart Things Hub which I will use to connect any Z-Wave devices. I would prefer to move away from third party cloud-based Gateways such as the 2 above, I am following this thread (https://community.home-assistant.io/t/zigbee2mqtt-getting-rid-of-your-proprietary-zigbee-bridges-xiaomi-hue-tradfri/52108) with interest currently and plan to move over to this platform removing the need to use the Xiaomi Gateway altogether.</p>
<hr --- </hr>

| [Xiaomi Gateway](https://www.banggood.com/Original-Xiaomi-Upgrade-Smart-Home-WiFi-Remote-Control-Multi-functional-Gateway-p-1047282.html?rmmds=search) | [Zigbee](http://www.zigbee.org/what-is-zigbee/) | [SmartThings Hub](https://www.amazon.com/Samsung-SmartThings-Smart-Home-Hub/dp/B010NZV0GE) | [Z-Wave](http://www.z-wave.com/) |
| --- | --- | --- | --- |
| <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Xiaomi%20Gateway.jpg" width="250"/> | <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Zigbee.png" width="250"/> | <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Samsung-Smart-Hub-1.jpg" width="250"/> | <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/ZWave.png" width="250"/> |

<h4 align="left">Zigbee Gateway:</h4>
<p align="left">As stated above I use the Xiaomi Gateway as a bridge for all of my Xiaomi family of Zigbee and Wi-FI based sensors into HA. It has a not so friendly to use App and all spoken commands are in Chinese. It does intergrate with its ecosystem ok, with support for using its switches as door bells and playing a sound it also has a rgb led which will change colours on events like smoke detection it turns red or alarm trigger.</p>
<h4 align="left">Z-Wave Gateway:</h4>
<p align="left">I bought a Smart Things Hub at the same time I purchased my Echo whilst I was in the USA, I had intended to use it as the bases of my smart home but once again there was no support for the Australian market at the time and there still is no word of it being released here. I keep it around as one of the things on my list still to integrate is my front door lock and the security protocols on most Door locks don’t work directly with HA, but they will with Smart Things. Also, most door locks seem to use Z-Wave protocol, the frequencies for Z-Wave differ for Australia from the USA (here in Australia that part of the spectrum is used by a cellular carrier), so I will need to change it anyway. So, now it’s a white brick occupying space in my data rack and network I am hoping I can find a decent Wi-Fi/Bluetooth Door lock and can do away with it altogether.</p>
<hr --- </hr>
<hr --- </hr>

<h3 align="left">Sensors</h3> 

| <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Xiaomi%20Logo.png" width="150"/> | <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Sonoff%20Logo.png" width="200"/> |
| --- | --- |

<p align="left">My first foray into the home sensor market was with Sonoff, they needed to be hacked to use them with HA and I found them not very accurate. I found a lot of chatter on the HA Forums about these cheap sensors out of China that not only integrated well with HA they worked well also. Xioami are a kind of supermarket of many products some of which they wrap up into their smart device eco system called Mi. These devices can be purchased from a few sites the best I found was Banggood and GearBest, there shipping was quick on most things and their packaging is professional, so items are well protected.</p>
<hr --- </hr>

| [Motion Detector](https://www.banggood.com/Original-Xiaomi-Smart-Home-Aqara-Human-Body-Sensor-ZigBee-Wireless-Connection-7m-Detection-Distance-p-1177007.html?rmmds=detail-top-buytogether-auto__2&cur_warehouse=CN) | [Door & Window Sensor](https://www.banggood.com/Original-Xiaomi-Intelligent-Door-Window-Sensor-Control-Smart-Home-Suit-Kit-Accessory-p-1017541.html?rmmds=detail-top-buytogether-auto__3&cur_warehouse=CN) | [Smart Switches](https://www.banggood.com/Original-Xiaomi-Smart-Home-Suit-Accessories-Mini-Smart-Wireless-Switch-Button-p-1049175.html?rmmds=detail-top-buytogether-auto__4&cur_warehouse=CN) | [Temperature Sensor](https://www.banggood.com/New-Arrival-Original-Xiaomi-Aqara-Intelligent-Smart-Home-Temperature-Humidity-Sensor-Set-White-p-1148666.html?rmmds=detail-top-buytogether-auto__5) |
| --- | --- | --- | --- |
| <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Motion%20Sensor.jpg" width="250"/> | <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Door%20Sensor.jpeg" width="250"/> | <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Smart%20Switches.png" width="200" height="250"/> | <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Temp%20Sensor.jpg" width="250"/> |

<h4 align="left">Motion Sensors:</h4>
<p align="left">I have placed motion sensors in every room of my house as well as at the entrance to my property (facing the front door) and a few at the rear. I use external sensors as motion light sensors they turn on the front and rear lights upon motion detect. The interior ones in the playroom, laundry and bathrooms are also used to turn lights on and off with motion as I found my family just leave these lights on all day. I also use them for unauthorized motion detection once the alarm has been set to trigger TTS to warn intruder that alarm has been triggered and to get the f*** out as police have been notified, as well as set in motion the alarm sequence. I hope to start to also utilize these in conjunction with other methods to introduce room detection/presence.</p>
<h4 align="left">Door & Window Sensors:</h4>
<p align="left">I have placed Door & Window Sensors on everything that opens & shuts that I want to know the status of. I use these tell me if there is an open door/window when we are trying to arm the alarm, if there is, a notification is played over the speakers to tell me "X" window is still open would you still like to set the alarm. They are also used to alert of unauthorized access and set in motion alarm sequence if its armed.</p>
<h4 align="left">Smart Switches:</h4>
<p align="left">I have a few of these around the place and a bunch more waiting to find a use for. The reason I got these was once I connected the ceiling fans to a 4ch Sonoff (more on these later) I disconnected the wall switch for the fans. This drove my wife crazy having to turn the fans on and off via her phone (lots of swearing and you need to rip this f*&^%$# smart home crap out), so I purchased about 10 or so of these Xiaomi Smart Switches. I use them to on single click cycle which upon a single click, it cycles through increasing the fan speeds and last one turns it off. I also use one at the entrance as a door bell which is used in several automations one for recording of ip camera and displaying it on the alarm panel screen by the front door. If we are watching TV/Movie it pauses what we are watching (Cable or Kodi) and turns the lights up displays who is at the front door from a snapshot taken with the camera recording. I also have one in the entertainment area for manually turning the (20) Edison bulbs on/off and fairy lighting modes. These switches have single click, double click and long press modes so can be used to trigger several automations of the one unit.</p>
<h4 align="left">Temperature & Humidity Sensors:</h4>
<p align="left">I have one of these in every room of the house as well as one located in the entertaining area out the back of the house. I use them mainly to tell me the temperature but do use them to trigger automations around when to turn on the bathroom heating and with a moisture sensor in the shower to trigger the exhaust fan. These are also used to control the climate in the bedrooms of a night time, not really for the main living areas.</p>
<hr --- </hr>
<hr --- </hr>

<h3 align="left">Fan & Lighting Control</h3> 

| <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Xiaomi%20Logo.png" width="150"/> | <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Sonoff%20Logo.png" width="200"/> |
| --- | --- |

<p align="left">I like many others use Sonoff single, daul and 4ch switches to control the power to my lights over Wi-Fi. These units need to be flashed with firmware (plenty of info out there on how to do it, I used Tasmota Firmware). I have placed all of my switches behind the wall plate (Gyprock walls) had to make fairly large holes to accomodate the 4ch model but can always plaster it back up afterwoods(took me about 2 months of nagging to sand the patches and re paint walls).</p>
<hr --- </hr>

| [Sonoff Basic](http://sonoff.itead.cc/en/products/sonoff/sonoff-basic) | [Sonoff Dual](http://sonoff.itead.cc/en/products/sonoff/sonoff-dual) | [Sonoff 4CH](http://sonoff.itead.cc/en/products/sonoff/sonoff-4ch) | [Sonoff RF Bridge 433](http://sonoff.itead.cc/en/products/appliances/sonoff-rf-bridge-433) |
| --- | --- | --- | --- |
| <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Sonoff%20Basic.jpg" width="250"/> | <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Sonoff%20Dual.jpg" width="250"/> | <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Sonoff%204ch.jpg" width="250"/> | <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Sonoff%20RF%20Bridge.jpg" width="250"/> |

<h4 align="left">Light Switches:</h4>
<p align="left">I use the Sonoff Basic & Dual for single and dual wall switches respectively and these are pretty straight forward flashed with Tasmota Firmware and added to HA via the MQTT Switch component. I installed all of these switches behind the existing wall plates and connected the original switch to the available gpio pins on the board.</p>
<h4 align="left">3 Speed Ceiling Fans:</h4>
<p align="left">I use the Sonoff 4Ch again flashed with the same firmware and I connected first ch to the high speed of the fan, 2nd & 3rd ch are connected to the med and low via a 6uf capacitor. The last channel is connected to the light switch again I used the gpio pin to connect the board to the wall plate, so the light can still be controlled via the wall switch. These can now be voice controlled via Alexa turn fan on/off turn fan speed to low, medium & high.</p>
<img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Fan%20CCT.png"/>
<h4 align="left">Garage Door:</h4>
<p align="left">I have an RF controlled relay connected to my garage door opener and I use the Sonoff RF Bridge to control it. I also have a Xiaomi Door Sensor to tell me whether the garage door is open. At the moment I use a Xiaomi smart switch located in the garage to control the door whilst I’m in there "Single Click" up, down and stop, "Double Click" Garage Light, Long Click manual up and down this way I can adjust how open I would like the door to be if I’m working in there. I wish to add a Bluetooth beacon to introduce geofencing to have the door open automatically when we are arriving home but atm there isn't enough room to fit the car due to my abundance of toys I no longer use.</p>
<hr --- </hr>
<hr --- </hr>

<h3 align="left">LED Lighting</h3> 
<img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Xiaomi%20Logo.png" width="150"/>
<p align="left">I have a few RGBWW strips around the house used mainly for mood lighting aswell as practical lighting on the staircase. These are all controlled by MiLight Wi-FI LED controllers with appropriate power supplies.</p>
<hr --- </hr>

| [5m RGBWW LED Strip](https://www.banggood.com/5M-RGBW-RGBWW-4-In-1-SMD5050-300LEDs-Strip-Light-Non-waterproof-Indoor-Use-DC12V-p-1155159.html?rmmds=myorder) | [LED Power](https://www.banggood.com/AC100-240V-To-DC12V-6A-72W-Power-Supply-Adapter-for-LED-Strip-Light-p-1111858.html?rmmds=myorder) | [Mi Light Wi-FI Controller](https://www.banggood.com/Mi-Light-24A-DC12-24V-2_4G-RF-4-Channel-RGB-LED-Remote-Controller-p-968820.html?rmmds=myorder) | [LED Diffuser](https://www.banggood.com/3050CM-XH-U1-U-Style-Aluminum-Channel-Holder-For-LED-Strip-Light-Bar-Under-Cabinet-Lamp-Lighting-p-1142676.html?rmmds=myorder&cur_warehouse=CN) |
| --- | --- | --- | --- |
| <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/LED%20Strips.jpg" width="250"/> | <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/LED%20PSU.jpg" width="250"/> | <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/Mi%20Light.jpg" width="250"/> | <img src="https://github.com/JamesMcCarthy79/Home-Assistant-Config/blob/master/HA%20Pics/LED%20Diffuser.jpg" width="250"/> |

<h4 align="left">Staircase Lighting:</h4>
<p align="left">I have 80cm LED strips on the underside of each step installed with a LED Diffuser the steps are split by 2 Mi Light Wi-Fi controllers. I have all odd stairs on one controller and all even on the other so I can have the colours alternate when its a special occasion or seasonal holiday. Their standard setup is to turn on (warm white) 30mins after sundown and turn off with the activation of the bed time script. Once the bed time script kicks in the Staircase LED strips are set to turn on only during motion detection of the motion sensor at the top of the stairs, they turn off again 5 mins after last motion detecion. Each alternate strip is soldered together and placed into a channel countersunk in to the step which is then covered by bamboo floor boards. The strips themselves are installed on the underside of the step overhang so they face back towards the step below it was a massive job (lots of swearing) and now all cabling is hidden it looks great and effect when stairs are light is awesome really makes the staircase a feature of the house. Each strip works out to be around 5.6m in length so I decided to power them sufficienatly with 12v 6A 72W PSU.</p>
<h4 align="left">LED Back Lighting:</h4>
<p align="left">I purchased 3 x 5m LED strips to do the stiarcase mentioned above and had about 3.5m left after the project was complete so rather then let them go to waste (like they were ever going to be) I decided to place a few strips behind my PC Monitor, Media TV, Bedroom TV and Entertaining TV. Each strip is controlled by the Mi Light Wifi LED controller and on normal nights they just give a soft blue glow from behind the screens. When music is playing I found a project where they had a script which would change the LED colour to match that of the Album artwork that was playing at the time. I also aim to port this across to work with Kodi and the TV Show/Movie Poster colours.</p>
<hr --- </hr>
