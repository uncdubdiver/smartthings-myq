# dbdevelopment-smartthings-myq
My personal setup for the MyQ garage door opener integration for SmartThings

### Pre-requisites
Must have a Samsung SmartThings account setup (https://account.smartthings.com)
Must have a MyQ account setup (https://myqchamberlain.com)

### To integrate this into SmartThings, you'll follow these steps:
Start by logging into to your SmartThings account

### 1. My Device Handlers
1. Navigation, click on _My Device handlers_.
2. Click on [+ Create new Device handler].
3. Select the _From Code_ tab.
4. Copy and paste in the code from the devicetypehandler.txt file.
5. Click [Create].
6. Once the page reloads, towards the top right corner, click [Save].
7. Click [Publish] -> [For Me].

#### 2. My Devices
1. Navigation, click on _My Devices_.
2. Click [+ New Device].
3. Create the new device as such:
- Name: MyQ Garage Door Opener
- Label: MyQ Garage Door Opener
- Zigbee Id: <blank>
- Device network Id: myq01
- Type: DB Dev - MyQ Garage Door Opener
- Version: Published
- Location: Home
- Hub: SmartThings Hub
- Group: <blank>
4. Then click [Create].
5. Once the page reloads, scroll down to the Preferences row and click [edit].
6. Populate your MyQ Username/Email Address and MyQ Password, then click [Save].

### Test MyQ Device Setup
1. Navigation, click on _My Device Handlers_.
2. Click on _dbdevelopment : DB Dev - MyQ Garage Door Opener_.
3. On the top right side, click [Simulator <].
4. For Location, select _Home_, then click [Set Location].
5. For Preferences, for Choose a device to test with, select _MyQ Garage Door Opener_, then click [Install].
6. You'll be presented with the following buttons:
- Refresh: [refresh]: this button will query the status of your garage door (open, closed)
- Door Control: [open] [close]: these buttons will either open or close your garage door opener
- Garage Door Contrl: [open] [close]: basically the same thing as Door Control
- Health Check: [ping]: option which is setup ActionTiles to work properly
- Raw: comment window: nothing to do here
If all of your tests work properly above, then you should be GTG to add this to your SmartThings app.

### DISCLOSURE
I am not SmartThings developer, I just did this because I couldn't get the other (way more advanced) MyQ garage door opener SmartApp that's out there to work with my system, so I created one myself.  It works well for me and this isn't for sale, so feel free to use it, tweak it, whatever you want!
Also, the apps seems to _look better_ in the Classic app.  For some reason, the new SmartThings app has a lot of extra settings that I can't seem to get rid of, but it should still work as expected!

Enjoy!
