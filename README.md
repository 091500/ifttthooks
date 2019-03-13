## IFTTT Hooks - standalone app and widget for Samsung smartwatch series

Send IFTTT webhook events from your wrist

video [presentation](https://www.youtube.com/watch?v=vmenfESsaJg)

**Features:**

* Galaxy Watch support
* Color picker for widget slots
* 6 widget slots
* Import key feature


### Requirements
1. visit [ifttt.com](http://ifttt.com) and obtain webhook key.
1. create an applet which uses webhook
1. install IFTTT Hooks app from Samsung Galaxy Apps Store on your watch and setup it


[<img width="250" src="https://github.com/091500/ifttthooks/blob/master/GalaxyStore_English.png?raw=true">](https://galaxy.store/ifttt)


### App menu and configuration
App main menu consists of the following items:

➊ **Send Triggers** - send Triggers to your IFTTT applets.

➋ **Setup Keys** - add or delete your keys.
Required fields: 
- Name
- Key

➌ **Setup Triggers** - add or delete your Triggers.
Required fields: 
- Name
- Key
- Event Name
- Widget Slot

➍ **Setup Widget** - assign Triggers to Widget slots.

➎ **Widget Colors** - assign colors to Widget slots.

   
   
### App widget
App has a built-in Widget with **six** slots: 12h, 2h, 4h, 6h, 8h, 10h.
Custom Trigger could be assigned to each slot.

   
   
### Import Key feature
This outstanding feature allows to quickly import long key strings instead of typing them on your watch!    
Make sure your watch is connected to internet. Then perform the following steps:    
1. visit [IFTTT Hooks Import Key service](https://murmuring-escarpment-62267.herokuapp.com)
2. generate short 4-symbol code for your key   
3. open IFTTT Hooks app and go to Setup Keys ⇨ Add ⇨ Import Key   
4. enter generated 4-symbol code and enjoy   

In case something goes wrong you will see an error message.

### Network connection
App uses network connection only to send requests when you press widget slot 
buttons or choose an item from Send Triggers list.

Send Triggers menu item shows a notification if network connection is absent on your device.

You are able to use app even without WiFi connection. In this case your smartwatch should be connected to your phone over bluetooth. 
Bluetooth internet tethering should be enabled in your phone Connection Settings.

Bluetooth tethering on Android:   
<img src="https://github.com/091500/ifttthooks/blob/master/Android-mobile-hotspot-setup.png?raw=true">



### Short quiz, please answer
[IFTTT Hooks quiz](https://goo.gl/forms/Muml6iXiLzn5xjMI2)


Share your impressions with #IFTTTHooks hashtag

Thank you

### Version history
2019.01.15 release date :sunglasses:    
2019.02.14 Delete Trigger fixed
