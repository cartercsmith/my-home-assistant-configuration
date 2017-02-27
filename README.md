# My Home Assistant configuration

**Sharing my HASS configuration for two main reasons:**
  - Studying, copying and modifying other users configurations was a great help when I started using HASS
  - Looking forward to improvement suggestions from other users

**Current automations:**
  - automatic broadcast of TTS alerts in the morning when travel time to work exceeds a certain duration
  - automatically turn off all devices when the last person leaves the house
  - automatically turn on favorite music of each user when arriving home
  - automatically turn on/off specific light scenes based on the time of the day
  - automatically turn on/off nightlamps at night, when going to bed
  - wake up with an all-in-one morning routine (light scenes, music, radio news broadcast, weather forecast, ...)
  - control different audio media-players through one user interface (on/off - devices - presets - volum control, ...)
  - automatically modify light scenes when playing/stopping different video media-players
  - automatically receive TTS reminders, per user (when present) or for all users in the household
  - motion triggered lights in bedroom

Check out the screenshots folder a view on the UI.
  
**Setup:**
  - Raspberry Pi 3 (Complete Starter Kit - 32 GB edition)
  - Hassbian
  - PostgreSQL database

**Household situation:**
  - 2 users (Benoit & Jurgen)
  - rooms:
    - living room (lights, media players)
    - bedroom (lights, media players)
    - bathroom (media player)
  - device tracking via iPhone, by using:
    - NMAP
    - Owntracks (GPS), combined with MQTT through cloudMQTT
    - iBEACONS (trigger IFTTT maker channel via Beecon IOS app)
    - iCLOUD (not used currently because 2-factor authentication not supported)
    
**Hardware devices installed:**
  - Lights: Philips Hue (color, white, go, led, etc..) & Flux WiFi Smart LED Light Bulbs
  - Thermostat: Nest
  - Motion sensor: Zwave multisensor 
  - iBeacons: estimote (not used currently because no reliable results)
  - Media-players: Bose SoundTouch, Apple TV, Google Home, Chromecast & Chromecast audio
    
**Components used:**
  - automations
  - alerts
  - scripts
  - groups:
    - non-default home
    - hiding/showing certain groups based on conditions
    - tab dedicated to mobile view
  - zones:
    - home
    - multiple circles around home for proximity
    - workplace both users
  - scenes
  - sensors & binary sensors: 
    - google travel
    - uber
    - synology
    - yr / darksky
    - sun / moon
    - template
    - input select, boolean & slider
    - device-tracking
  - proximity
  - tts (google)
  - emulated hue (google home)
  - notify (telegram & instapush)
  - plex
  
**On the to-do list:**
  - Microlocation (reliably knowing who is in which room):
    - Understanding why the iBEACON setup fails
    - Waiting for my HappyBubbles devices to arrive to explore alternatives for microlocation
  - Reboot through shell command (root issue)
  - Append text containing template values to text file (root issue I think)
  - Relevant automations (beyond the fun to implement them, also actually useful)
  - Sleep more again...

!!! Help/suggestions welcome !!!

**Some links:**
  - www.canakit.com
  - www.amazon.com/gp/product/B00SGLKWQW/ref=oh_aui_detailpage_o01_s00?ie=UTF8&psc=1
  - www.beaconsandwich.com
  - www.estimote.com
  - www.happybubbles.tech


  
