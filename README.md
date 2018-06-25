# Access Point Finder

This is something I made during a weekend to see if a directional antenna and a raspberry would be able to pinpoint an access point

## How it works

There are 2 equipment involved in this test. One is a raspberry pi 3B with an USB network interface and a directional antenna and the second is an ESP8266 that runs as an AP. The code has been modified to lower the power output.

### RPI

RPI also has an OLED screen that displays the power output and if there is no signal

## What is next

I want to change the raspberry for another ESP8266 or a another C++ based device that would be able to scan faster and I also want to get another antenna that would be compact (for this test I used an outdoor antenna which was quite large)

## Known Issues

The linux stack has quite a big delay, refreshing the signal power on a direction gradually in 5 seconds, that is a lot is you want something compact that will scan fast (imagine scanning 5 seconds in each direction and then making a decision. this may work for a radar but not for a person) and I assume that an ESP would be much faster.
