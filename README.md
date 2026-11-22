# FlightWatch — Live Flight Tracker

**A live map of aircraft over North America and nearby areas.**
Open `index.html` in a browser. It needs internet.

## What it does
Shows real aircraft positions on a dark map, with details such as altitude, speed, heading and climb rate, plus airline names from call-sign codes (e.g. UAE = Emirates). It refreshes on a timer.

## How it works
- **Data:** the OpenSky Network's free API, with no key.
- A bounding box (latitude and longitude limits) asks only for aircraft in this area.
- Each aircraft comes back as a list of numbers, such as position, velocity, track and vertical rate. The code reads each one by its position in the list.
- **Map:** Leaflet.js, styled dark with a CSS filter.

## Limits (honest)
- OpenSky limits how often anonymous users can ask. If it shows an error or empty map, wait and retry.
- Coverage depends on volunteer receivers, so some areas have gaps.
- Not for navigation or safety use.

## Connection to my other work
This is the same kind of aviation interest as my Airbus Beluga project: [Beluga Cargo](https://github.com/TechTonicCortex/beluga-cargo-visualiser).

## What I learned
Reading data from a list by index, handling API limits, and updating a map without reloading the page.

## Next steps
Click a plane to follow it, and show the Beluga when it flies (call sign search).

---
Part of [Aadit's projects](https://github.com/TechTonicCortex/techtoniccortex).
