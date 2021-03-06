# VRChatOSCSwitch
Ever wanted to run multiple OSC apps at once while playing VRChat?<br />
If so, you might know that VRChat will not communicate with multiple apps on the same UDP ports (9000 and 9001), mostly because these same apps like to lock the ports, which will make them unavailable for other apps that are trying to communicate with VRChat.<br />
VRChat itself is able to receive messages from multiple apps on the same ports, but the way the apps implement OSC support can lead to issues like this.

This is why I created this app, which will act as a "switch" between the OSC apps (VRCFT, YeelightOSC etc.) and the target app (VRChat), making life easier for both sides.

This is how the program works:<br/>
![diagram](https://i.imgur.com/7Y0KDit.png)

## How to set up the program
For more information, take a look at the wiki here: https://github.com/KaleidonKep99/VRChatOSCSwitch/wiki/VRChatOSCSwitch-guide

## Dependencies
- [Costura.Fody](https://github.com/Fody/Costura) by Fody.
- [Newtonsoft.Json](https://www.newtonsoft.com/json) by Netwonsoft.
- [Bespoke.Osc](https://opensoundcontrol.stanford.edu/implementations/Bespoke-OSC.html) by matt from Standford University.
