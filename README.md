# Ring Keypad as Garage Door Keypad

Home Assistant blueprints to easily configure a Ring Keypad V2 as an external keypad for operating your garage door. 

There are two flavors:
1) **Keymaster** - This Blueprint will validate the codes entered into the keypad against those of your Keymaster codes that are currently active. Learn more about [KeyMaster](https://github.com/FutureTense/keymaster) here.

   [![Add Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)]( https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A//github.com/Fiercefish1/RingKeypad_GarageDoorOpener/blob/main/GarageDoorKeypad_Keymaster.yaml)

2) **String** - This Blueprint allows you to provide a string of code combinations for the keypad to validate against. If you don't use Keymaster and want to just provide a few codes for the opener, you can do that here.

   [![Add Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)]( https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A//github.com/Fiercefish1/RingKeypad_GarageDoorOpener/blob/main/GarageDoorKeypad_String.yaml)


## Features
* Toggles any cover (e.g. garage door) when a valid code is provided
* Choose which button/s toggle the cover after valid code entry (e.g Disarm button opens door #1, Armed Home buttom opens door #2)
* Can use existing users and codes from Keymaster
* Can be configured multiple times to control multiple garage doors
* Create your own custom actions for Fire, Police, Medical buttons (must be held for three seconds)

## Prerequisites
1. A Ring Keypad V2 connected via Z-wave to Home Assistant
2. A cover that you want to control.

## Keypad Mounting
WIth the help of some velcro, minus the back plate, the keypad fits perfectly inside of [this dual-gang weather proof cover](https://www.amazon.com/gp/product/B001JEPX5I), for $9.00 on Amazon. 

<img src="keypad-box-2.jpg" width="300"> <img src="keypad-box.jpg" width="300"><img src="keypad-in-box.jpeg" width="300">

