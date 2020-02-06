## IFTTT Hooks - standalone app and widget for Samsung smartwatch series

Send IFTTT webhook events from your wrist

video presentation on YouTube:    
[<img width="450" src="https://github.com/091500/ifttthooks/blob/master/scr.png?raw=true">](https://www.youtube.com/watch?v=vmenfESsaJg)


**HOWTO, Setup full guide (PDF)**  →  [HERE](https://github.com/091500/ifttthooks/blob/master/guide-final-en.pdf?raw=true)  ←

**Configuration Service - how to create config - full guide (PDF)**  →  [HERE](https://github.com/091500/ifttthooks/blob/master/create_config.pdf?raw=true)  ←

**Configuration Service - how to load config - full guide (PDF)**  →  [HERE](https://github.com/091500/ifttthooks/blob/master/load_config.pdf?raw=true)  ←

**Services**     
[IFTTT Hooks Import Key service](https://murmuring-escarpment-62267.herokuapp.com)     
[IFTTT Hooks Configuration Service](https://murmuring-escarpment-62267.herokuapp.com/app_configurations)     

**Features:**

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

**Warning: do not use any special characters and spaces for 'Event Name'. Your trigger may not work.**    
Bad: Open Garage    
Good: open_garage    
     
Bad: Party & Lights   
Good: party_lights   
    
Why? because when you do so, the url will be escaped. See the difference:    
Bad: Party & Lights    
URL: https://maker.ifttt.com/trigger/Party%20%26%20Lights/with/key/your_key   
    
Good: open_garage    
URL: https://maker.ifttt.com/trigger/party_lights/with/key/your_key    


➍ **Setup Widget** - assign Triggers to Widget slots.

➎ **Widget Colors** - assign colors to Widget slots.

➏  **Reset Config** - reset app configuration on watch.

➐  **Load Config** - load config from Configuration Service by code.

➑ **Upload Config** - upload current app config to the Configuration Service.

   
   
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
**Warning: for security reason code will expire in 10 minutes**


### Configuration Service
This outstanding feature allows to do the following things:
1. Create and test Configuration     
2. Import Configuration on your watch         
3. Export Configuration to a backup file         
4. Create configuration from a backup file        

Open the following link in your desktop browser:            
1. [IFTTT Hooks Configuration Service](https://murmuring-escarpment-62267.herokuapp.com/app_configurations)     
2. fill in required information and create configuration        
3. test your webhooks by pressing Try buttons        
4. save configuration (remeber the code)    
5. save backup file     

Tap on **Load Config** in the app menu:    
1. provide code        
2. import configuration on your watch       

Tap on **Upload Config** in the app menu:    
1. remeber code            
2. visit [IFTTT Hooks Configuration Service](https://murmuring-escarpment-62267.herokuapp.com/app_configurations)     
3. provide code     
4. load config     
5. save backup file     

In case something goes wrong you will see an error message.     
**Warning: for security reason code will expire in 10 minutes**

### Internet connection (Watch MUST have Internet connection on to send triggers)
App uses Internet connection only to send requests when you press widget slot buttons or choose an item from Send Triggers list.

Send Triggers menu item shows a notification if Internet connection is absent on your device.

You are able to use app even without WiFi connection. In this case your smartwatch should be connected to your phone over bluetooth. 
Bluetooth Internet tethering should be enabled in your phone Connection Settings.

Bluetooth tethering on Android:   
<img src="https://github.com/091500/ifttthooks/blob/master/Android-mobile-hotspot-setup.png?raw=true">



### Short quiz, please answer
[IFTTT Hooks quiz](https://goo.gl/forms/uj9VaQ6ZRWKB4Rhz2)



### FAQ (udpated 2019-06-20)

Q: **Can I feel some kind of feedback when pressing widget buttons?**    
A: Visual feedback was added in version 1.0.8   
Tizen Platform has certain limitation for widgets. There is no way to make a vibration or sound on widget screen: [https://developer.tizen.org/development/guides/web-application/application-management/applications/widget-application](https://developer.tizen.org/development/guides/web-application/application-management/applications/widget-application)

Q: **I cannot enter code, because input field does not display first letters of text. How do I enter the text?**    
A: This was fixed in version 1.0.7   
Some users have words suggestion turned on in their Keyboard settings. A quick workaround could be turning off the suggestions, or simply swipe left on the text input field:
[https://developer.samsung.com/galaxy-watch/design/patterns/input](https://developer.samsung.com/galaxy-watch/design/patterns/input)

Q: **When I trigger action there is a delay**    
A: Some users may notice a delay after they trigger an action. This is not caused by app. Network connection, as well as IFTTT cloud servers may cause delay.    


### If App does not work

Some users instead of sorting out the problem post negative comments immideately. This is not a clever approach. In case you faced a problem and the app 'does not work' refer to the following checklist:   
1. read carefully setup guide [here](https://github.com/091500/ifttthooks/blob/master/guide-final-en.pdf?raw=true)  
2. test your webhook in desktop web browser: open [https://ifttt.com/maker_webhooks](https://ifttt.com/maker_webhooks) then click on 'Documentation' link   
3. successful result in prevous step? NO: go to item 2, YES: go to item 4   
4. setup the app correctly on Watch   
5. check Internet connection on Watch   
6. successful result in prevous step? NO: go to item 5, YES: go to item 7 
7. Internet connection is present on Watch, App is configured correctly, IFTTT Webhook works in destktop browser, Trigger is sent successfully from IFTTT Webhooks watch app?
8. successful result in prevous step? YES: GONGRATULATIONS, YOU ARE GREAT!, NO: go to item 9 
9. submit an issue [here](https://github.com/091500/ifttthooks/issues), provide detailed information on your problem (please mask your IFTTT keys and any private information)



### Some of Buyers' comments and ratings
<img width="700" src="https://github.com/091500/ifttthooks/blob/master/1.png?raw=true">    
<img width="700" src="https://github.com/091500/ifttthooks/blob/master/2.png?raw=true">    
<img width="700" src="https://github.com/091500/ifttthooks/blob/master/3.png?raw=true">    


Share your impressions with #IFTTTHooks hashtag

Like the App?  Please leave a feedback on Samsung Galaxy Store and rate the app.    

Thank you!

### Version history
2019.01.15 release date :sunglasses:    
2019.02.14 v.1.0.6 Delete Trigger fixed   
2019.04.02 v.1.0.7 Input fields display fixed   
2019.06.11 v.1.0.8 Added visual feedback on widget button press   
2019.12.20 v.1.0.9 Improvements:    
  Added sorting (a-z) in Send Triggers, Setup Triggers, Setup Keys lists.    
  Added App shortcut on widget screen.    
  Improved Import Key Service server response.    
2020.02.04 v.1.0.10 Added Reset/Load/Upload config support    
