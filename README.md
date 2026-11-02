# Time to Step Out

San Francisco weather changes through the day. By the time you're free, a nice afternoon can turn windy and grey. **Time to Step Out** tells you when it's genuinely great outside, so you can get off your screen and enjoy it.

This is an early prototype for the Pacific Heights / Alamo Square area.

## What it does

- Checks the live hourly forecast for today and tomorrow
- Finds the stretches of great weather
- Shows the updates you'd get, at most two a day and at least 2½ hours apart. Each one says:
  - how long the good weather should last, as a range (e.g. "about 3–4 hours")
  - what will end it (wind picking up, fog rolling in, cooling down, sunset)
  - why it's great (temperature, wind, sky, rain chance)
- Sends nothing on days without great weather

## What counts as great

- 60–76°F
- Wind under 14 mph, gusts under 20 mph
- Under 40% chance of rain
- No fog (clouds are fine)

These limits were tuned from 14 real outings that felt great.

## Try it

It's a single HTML file with no install, accounts or backend.

1. Download [`index.html`](index.html)
2. Open it in your browser

It needs an internet connection to load the forecast.

## How it works

- Forecast data comes from [Open-Meteo](https://open-meteo.com/), a free weather API that needs no key
- Everything runs in your browser, and nothing is stored or sent anywhere else

## Status

A prototype for testing the idea. Updates appear on the page as phone-style notifications; no real emails or push notifications are sent yet.
