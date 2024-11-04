# Ring Keypad Blueprints for Home Assistant

Home Assistant blueprints to easily configure a Ring Keypad V2 as an external keypad for operating your garage door, or controlling the Alarmo integeation using user-codes managed by Keymaster. 

*These blueprints were derived from the great work by [@imsorrybutwho](https://github.com/ImSorryButWho/HomeAssistantNotes) for Ring keypads with the Alarmo integration.  


## Alarmo + Keymaster Blueprint
**Alarmo keypad with Keymaster** - Instead of having to manage two sets of codes for users in Alarmo and Keymaster, this blueprint will validate any code input events on the keypad against active Keyaster codes before executing the desired alarm action. 

 [![Add Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)]( https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A//https://github.com/Fiercefish1/RingKeypad_GarageDoorOpener/blob/main/keypad_alarmo_keymaster.yaml)

 
## Garage Door Opener Blueprints
  
1) **Garage Door Keypad with Keymaster** - This Blueprint will validate the codes entered into the keypad against those of your Keymaster codes that are currently active. Learn more about [KeyMaster](https://github.com/FutureTense/keymaster) here.

   [![Add Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)]( https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A//github.com/Fiercefish1/RingKeypad_GarageDoorOpener/blob/main/GarageDoorKeypad_Keymaster.yaml)

3) **Garage Door Keypad with String Codes** - This Blueprint allows you to provide a string of code combinations for the keypad to validate against. If you don't use Keymaster and want to just provide a few codes for the opener, you can do that here.

   [![Add Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)]( https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A//github.com/Fiercefish1/RingKeypad_GarageDoorOpener/blob/main/GarageDoorKeypad_String.yaml)

## Keypad Mounting
WIth the help of some velcro, minus the back plate, the keypad fits perfectly inside of [this dual-gang weather proof cover](https://www.amazon.com/gp/product/B001JEPX5I), for $9.00 on Amazon. 

<img src="keypad-box-2.jpg" width="300"> <img src="keypad-box.jpg" width="300"><img src="keypad-in-box.jpeg" width="300">







