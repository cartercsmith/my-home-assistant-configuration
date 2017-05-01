# My Home Assistant configuration

----------------------------------------------------------------------------
Latest news (April 30th)
----------------------------------------------------------------------------
The Happy Bubbles implementation seems pretty stable by now and and I start to trust the state of the beacons:
  - istubb beacons on our keyrings
  - estimote beacons in our laptop bag for work
  - kontakt.io card beacons behind the cover of our iphones (quite happy I found these as they seem to do the job well)

Furthermore, iOS app addition was a major recent change too.

The issues cauding 'timer out of sync' still seem to be there.   But overall my HA is pretty stable for the moment.
Still hoping to understand what can be done about it, so anyone who had similar issues but was able to solve them, feel free to contact me.
----------------------------------------------------------------------------

**Sharing my HASS configuration for two main reasons:**
  - Studying, copying and modifying other users configurations was a great help when I started using HASS
  - Looking forward to improvement suggestions from other users

**Current automations:**
  - automatic broadcast of TTS alerts in the morning when travel time to work exceeds a certain duration
  - automatically turn off all devices when the last person leaves the house
  - automatically turn on favorite music of each user when arriving home
  - automatically turn on/off specific light scenes based on the time of the day
  - motion based light in home office, with possiblity to overrule for 60 minutes using flic button
  - motion based light in bed room, using different scenes depending on the situation (someone sleeping or not) and overrule possibility with flic button
  - wake up with an all-in-one morning routine (light scenes, music, radio news broadcast, weather forecast, ...)
  - control different audio media-players through one user interface (on/off - devices - presets - volum control, ...)
  - automatically modify light scenes when playing/stopping different video media-players
  - automatically receive TTS reminders, per user (when present) or for all users in the household
  - automated 'manual' update of location new iOS app location depending on current situation/location

Check out the screenshots folder a view on the UI.

**Setup:**
  - Raspberry Pi 3 (Complete Starter Kit - 32 GB edition)
  - Hassbian
  - PostgreSQL database

**Household situation:**
  - 2 users
  - rooms:
    - living room (lights, media players)
    - bedroom (lights, media players)
    - bureau (lights)
    - bathroom (media player)
  - device tracking via iPhone, by using:
    - NMAP
    - Owntracks (GPS), combined with MQTT through cloudMQTT (bridged through Mosquitto)
    - Various beacons tracked with Happy Bubbles and MQTT_room for micro-location (currently testing)
    - iOS app

**Hardware devices & components installed:**
  - Lights: Philips Hue (color, white, go, led, etc..) & Flux WiFi Smart LED Light Bulbs
  - Thermostat: Nest
  - Camera: nest
  - Motion sensor: Zwave multisensor & Zooz 4-in-1 sensor
  - Beacons: estimote, istubb, Kontakt
  - Happy Bubbles
  - Flic buttons
  - MiFlora plant sensors
  - Media-players: Bose SoundTouch, Apple TV, Google Home, Chromecast & Chromecast audio
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
    - speedtest.net
    - systemmonitor
  - proximity
  - tts (google)
  - emulated hue (google home)
  - notify (telegram & instapush)
  - plex
  - flic
  - mqtt_room
  ...

**On the to-do list:**
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



