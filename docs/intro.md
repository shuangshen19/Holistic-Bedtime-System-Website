---
id: intro
sidebar_position: 1
---

# Introduction

## Narrative:
Our Hack is a design and prototype of an Automatic Bedtime Audio Playback System, which implicitly senses when a user goes to bed and responds by automatically playing their preferred audio to improve their sleep environment. The system hooks into Spotify to play music, podcasts, white noise, etc to users when they go to bed, but could additionally connect to smart home features like lamps or thermostats to turn off the lights and cool down the room during bedtime. When a user lays on their bed, we detect their presence with the ultrasonic rangefinder and pressure detector. Later on, we could incorporate the photoresistor and thermometer for sensing the room state.

## Abstractions:
### Simple:
When the user interacts with their bed, adjust the context of the room to support them falling asleep or waking by playing different audio tracks and adjusting the thermostat.

### Complex:
When bed occupancy changes from unoccupied to occupied (i.e. laying down), captured by an ultrasonic rangefinder, pressure detector, and/or other sensors, send a playback request to Spotify and other potential webhooks through IFTTT. Depending on the state of the room, captured by photoresistor and thermometer, optionally control the lights and temperature.


## Model:
<img style={{width: '80%'}} src={require("./img/model.png").default} />

## Prototype:
<img style={{width: '80%'}} src={require("./img/prototype.png").default} />