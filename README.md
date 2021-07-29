# feChallenge

## Brief
Melbourne weather is not awesome. build a page that *is* awesome that reports the current weather.
The page should show these weather conditions for the current location with a toggle for celsius/farenheit:
```
 ┌───────────────────┐
 │ CURRENT WEATHER   │
 │ 22° C | CLOUDS    │
 │ KEW, AUSTRALIA    │
 │                   │
 │ HUMIDITY  73%     │
 │ WIND      6.2 M/S │
 │ SUNRISE   05:41   │
 │ SUNSET    20:06   │
 │                   │
 │ [c]|[f] (toggle)  │
 └───────────────────┘
```
Throw it in a Github Repo (be sure to include any sources if preprocessing) or build it in your preferred online code playground (e.g. codepen, jsfiddle).

You can fetch the weather using a free API (details below). Get the current geo location using your preferred method (e.g. browser / ip lookup service). Fallbacks welcome.

As the API has a call limit the results should be locally cached (e.g. localstorage, cookie). When toggling c|f calculate the values instead of making another call.

Use Vue.js if possible, or your preferred framework, or simply pure JS... SCSS would be great, and some animation to make it hot (even when it's 8 degrees). The important thing is that the code is clean, consistent and crystal clear.

## API Details
Option 1: *Dark Sky*
 - API signup: https://darksky.net/dev/ (free signup, 1,000 requests/day, https support, must attribute dark sky)
 - Docs: https://darksky.net/dev/docs
 - Example call: https://api.darksky.net/forecast/YOUR_API_KEY/YOUR_LATITUDE,YOUR_LONGITUDE?exclude=minutely,hourly,alerts,flags

Option 2: *OpenWeatherMap*
 - Grab an API key here: https://openweathermap.org/appid (free signup, 60 requests/min, no https support!)
 - Docs: https://openweathermap.org/current
 - Example call: http://api.openweathermap.org/data/2.5/weather?lat=YOUR_LATITUDE&lon=YOUR_LONGITUDE&appid=YOU_API_KEY
