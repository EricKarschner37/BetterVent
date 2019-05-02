# BetterVent
A tablet-based reservation app written for Computer Science House.
<br>
<img src="https://raw.githubusercontent.com/WillNilges/BetterVent/master/app/src/main/res/mipmap-hdpi/logo.png" width="200" height="200">

# What is it?
BetterVent is a lightweight, open source, customizable android app that shows the status of conference rooms.
It has three main functions:
- Display the current event happening in a room as well as when the next event is

View when the room is free:

<img src="https://raw.githubusercontent.com/WillNilges/BetterVent/master/BetterVent_Screenshots/Screenshot_20190121_042312.png" width="50%" height="50%">

<img src="https://raw.githubusercontent.com/WillNilges/BetterVent/master/BetterVent_Screenshots/Screenshot_20190302-044311_BetterVent.jpg" width="50%" height="50%">

View when the room is reserved:

<img src="https://raw.githubusercontent.com/WillNilges/BetterVent/master/BetterVent_Screenshots/Screenshot_20190121_042156.png" width="50%" height="50%">

- Show a week-view interface of events for the next seven days

<img src="https://raw.githubusercontent.com/WillNilges/BetterVent/master/BetterVent_Screenshots/Screenshot_20190121_042504.png" width="50%" height="50%">

- A quick-mode function for ad-hoc events. Has an editable title field, as well as a name-list for queuing or attendance purposes

<img src="https://raw.githubusercontent.com/WillNilges/BetterVent/master/BetterVent_Screenshots/Screenshot_20190302-045308_BetterVent.jpg" width="50%" height="50%">

<img src="https://raw.githubusercontent.com/WillNilges/BetterVent/master/BetterVent_Screenshots/Screenshot_20190302-045456_BetterVent.jpg" width="50%" height="50%">

# How do I get it?
Currently, BetterVent is not on the Play Store, but you can download the .apk file in the releases tab.
(I'll try to keep it up to date)

# Future Features
- UI fixes
  - Adaptive layout that conforms to more screensizes
- Quality of life changes for Quick Mode
  - Add confirmation when leaving the fragment
  - Add button to clear Quick Mode without leaving the fragment
- Kiosk mode to prevent users from leaving the app
  - Device provisioning (make app admin?)
- Ability to filter events by keyword
- Settings panel
  - Event filtering
  - Colors
  
## Device Admin
To set the app as device admin (You need to do this before kiosk features work (Thanks, Google)) Connect to a computer and in the terminal (after installing adb) do this *BEFORE SETTING UP A GOOGLE ACCOUNT*:

```
adb shell
dpm set-device-owner --user current edu.rit.csh.bettervent/.AdminReceiver                                            
```