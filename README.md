# Ring Keypad Blueprints for Home Assistant

Home Assistant blueprints to easily configure a Ring Keypad V2 as an external keypad for operating your garage door, or controlling the Alarmo integeation using user-codes managed by Keymaster. 

*These blueprints were derived from the great work by [@imsorrybutwho](https://github.com/ImSorryButWho/HomeAssistantNotes) for Ring keypads with the Alarmo integration.  


### Keypad Performance
* By default the motion detector in the keypad has a reset timer of two seconds, which can cause it to flood the zwave network and make the keypad appear to have connection issues.  To address this you need  to go to the device page and update the configuration for parameter 26 Motion Sensor Timeout with a larger number (e.g. 30). 
* For the best connection, you'll want the keypad connected directly to the controller rather than hopping through other zwave relays (if possible). 


## Alarmo + Keymaster Blueprint
**Alarmo keypad with Keymaster** - Instead of having to manage two sets of codes for users in Alarmo and Keymaster, this blueprint will validate any code input events on the keypad against active Keyaster codes before executing the desired alarm action. 

 [![Add Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)]( https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A//raw.githubusercontent.com/Fiercefish1/RingKeypad_Blueprints/refs/heads/main/keypad_alarmo_keymaster.yaml)

 
## Garage Door Opener Blueprint
 
**Garage Door Keypad with Keymaster or User Provided Codes** - This Blueprint will validate the codes entered into the keypad against those of your Keymaster codes that are currently active, or against a string of codes you provide (if no Keymaster code sensors are detected). Learn more about [KeyMaster](https://github.com/FutureTense/keymaster) here.

[![Add Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)]( https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A//raw.githubusercontent.com/Fiercefish1/RingKeypad_Blueprints/refs/heads/main/GarageDoorKeypad_Keymaster.yaml)


## Keypad Mounting
WIth the help of some velcro, minus the back plate, the keypad fits perfectly inside of [this dual-gang weather proof cover](https://www.amazon.com/gp/product/B001JEPX5I), for $9.00 on Amazon. 

<img src="keypad-box-2.jpg" width="300"> <img src="keypad-box.jpg" width="300"><img src="keypad-in-box.jpeg" width="300">







