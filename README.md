# Python Weather Forecast
### version 1.0.0
Weather Forecast is a simple Python 3 console program to get Weather Forecast from DarkSky.net service API using any address as parameter. 

  - It uses Google Maps Geocoding API to transform any string address into numeric coordinates.
  - It obtains weekly forecast and related weather information for any coordinates in the World.
  - Output language and metric system are configurables parameters.

> Note: This program has been developed using Python 3.5.2. It's NOT compatible with Python 2.7 versions.

### Requirements

In order to get the weather forecast information from external services,you'll need to sign up and obtain your own API Key:
* Python 3.5.* installed in your OS.
* DarkSky.net API Key: You can obtain your own here: https://darksky.net/dev/
* Google Maps API Key - It's optional for development purposes, but you'll need to get your own key here: https://developers.google.com/maps/documentation/geocoding/get-api-key

### Configuration
You can change the main language for output information using ISO codes. By default, language variable (**LANG**) is "en". 

You can change the default code for **UNITS** variable that is "si" (International System). Available codes are: 
- **auto**: automatically select units based on geographic location
- **ca**: same as si, except that windSpeed is in kilometers per hour
- **uk2**: same as si, except that nearestStormDistance and visibility are in miles and windSpeed is in miles per hour
- **us**: Imperial units
- **si**: SI units (default)

You can find a list of available languages and unit codes here: https://darksky.net/dev/docs/forecast

### Usage
Once you have declared environment variables, you can execute the console program:

```sh
$ cd my-project
$ python3 forecast.py "Gran Via Street 28,Madrid"
```
And you'll get forecast information as output!:
![Output Example](http://ordermin.com/images/python-weather-forecast-output.png)

> Note: Forecast API is free until 1000 requests per day. For more information, check their FAQ: https://darksky.net/dev/docs/faq







