# Keypad Blueprints for Home Assistant

Home Assistant blueprints to use [KeyMaster](https://github.com/FutureTense/keymaster) codes with Alarmo via dashboard cards or a Ring Keypad V2. Also includes a blueprint to use the Ring Keypad v2 as garage door open using Keymaster or user provided codes.

*These blueprints were derived from the great work by [@imsorrybutwho](https://github.com/ImSorryButWho/HomeAssistantNotes) for Ring keypads with the Alarmo integration.  


### Ring Keypad Performance
* By default the motion detector in the keypad has a reset timer of two seconds, which can cause it to flood the zwave network and make the keypad appear to have connection issues.  To address this you need  to go to the device page and update the configuration for parameter 26 Motion Sensor Timeout with a larger number (e.g. 30). 
* For the best connection, you'll want the keypad connected directly to the controller rather than hopping through other zwave relays (if possible). 


## Alarmo with Keymaster codes
**For Alarmo custom lovelace card** - This blueprint allows you to use Keymaster codes on the digital keypad for [custom:Alarmo card](https://github.com/nielsfaber/alarmo-card), to control your Alarmo alarm. 
* Supports all Alarmo modes
* Logs the Code Slot # and the Alarmo alarm action to Logbook, to allow tracking of which users executed Alarm actions. 

 [![Add Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)]( https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A//raw.githubusercontent.com/Fiercefish1/RingKeypad_Blueprints/refs/heads/main/Alarmo_DashboardKeypad_Keymaster.yaml)

## Alarmo + Keymaster w/ Ring Keypad 
**Alarmo ring keypad with Keymaster** - Instead of having to manage two sets of codes for users in Alarmo and Keymaster, this blueprint will validate any code input events on the keypad against active Keyaster codes before executing the desired alarm action. 

 [![Add Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)]( https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A//raw.githubusercontent.com/Fiercefish1/RingKeypad_Blueprints/refs/heads/main/keypad_alarmo_keymaster.yaml)

 
## Ring Keypad Garage Door Opener
 
**Garage Door Keypad with Keymaster or User Provided Codes** - This Blueprint will validate the codes entered into the keypad against those of your Keymaster codes that are currently active, or against a string of codes you provide (if no Keymaster code sensors are detected). Learn more about [KeyMaster](https://github.com/FutureTense/keymaster) here.

[![Add Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)]( https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A//raw.githubusercontent.com/Fiercefish1/RingKeypad_Blueprints/refs/heads/main/GarageDoorKeypad_Keymaster.yaml)


## Keypad Mounting
WIth the help of some velcro, minus the back plate, the keypad fits perfectly inside of [this dual-gang weather proof cover](https://www.amazon.com/gp/product/B001JEPX5I), for $9.00 on Amazon. 

<img src="images/keypad-box-2.jpg" width="300"> <img src="images/keypad-box.jpg" width="300"><img src="images/keypad-in-box.jpeg" width="300">







