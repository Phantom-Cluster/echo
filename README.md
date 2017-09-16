# Alexa Controlling 8 Channel Relay With Node MCU v3

Before Using this code, Keep in Mind  :

 * Make Sure Arduino is Install On your System, and ESP8266 driver is also install.
 * By going tools you have set Correct Board which is Node MCU 12E 1.0
 
If You Accidently Fried Your Node MCU or Relay Please Don't Blame Me,
Code is Working Properly already 

You Need !
 * Node MCU v3
 * 8 Channel Power Relay.
 * Power Adapter to Turn On Node MCU Recommended 5v 1 Amp (Minimum)

And here's some code! where You Have to Make Changes :+1:

```javascript
//Change wifi before you flash
const char* ssid = "wifi Name";
const char* password = "Wifi Password";

//relay pin setup for funct
int relayOne = 5;
int relayTwo = 4;
int relayThree = 0;
int relayFour = 2;
int relayFive = 14;
int relaySix = 12;
int relaySeven = 13;
int relayEight = 15;


// Format: Alexa invocation name, local port no, on callback, off callback
lightOne = new Switch("Light One", 80, lightOneOn, lightOneOff);
lightTwo = new Switch("Light Two", 81, lightTwoOn, lightTwoOff);
lightThree = new Switch("Light Three", 82, lightThreeOn, lightThreeOff);
lightFour = new Switch("Light Four", 83, lightFourOn, lightFourOff);
outletOne = new Switch("Outlet One", 84,outletOneOn, outletOneOff);
outletTwo = new Switch("Outlet Two", 85, outletTwoOn, outletTwoOff);
outletThree = new Switch("Outlet Three", 86, outletThreeOn, outletThreeOff);
outletFour = new Switch("Outlet Four", 87,outletFourOn, outletFourOff);

//relay pins setup i Used D1,D2,D3,D4,D5,D6,D7,D8 followed as assigned below, if you are willing to change Pin or planning to use extra please Check Image in Github File..:)
    pinMode (5, OUTPUT);
    pinMode (4, OUTPUT);
    pinMode (0, OUTPUT);
    pinMode (2, OUTPUT);
    pinMode (14, OUTPUT);
    pinMode (12, OUTPUT);
    pinMode (13, OUTPUT);
    pinMode (15, OUTPUT);
    digitalWrite (5,HIGH);
    digitalWrite (4,HIGH);
    digitalWrite (0,HIGH);
    digitalWrite (2,HIGH);
    digitalWrite (14,HIGH);
    digitalWrite (12,HIGH);
    digitalWrite (13,HIGH);
    digitalWrite (15,HIGH);

```

If You Are Looking for  Channel Relay Coding for Alexa by Raspberry,[Check code on GitHub](https://github.com/Phantom-Cluster/Alexa-Raspberry-Single-Relay)


