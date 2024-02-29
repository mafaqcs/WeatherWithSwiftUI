
# iOS Weather App

This iOS weather application is designed to fetch weather data with the help of openweather API and displays it to the user in a clean and intuitive interface. Users can view the current weather conditions including temperature, min and max temperature, wind speed and pressure and other relevant information.

Additionally, the application allows users to refresh the weather data, retrieve weather data based on their current location using GPS, and manually enter a location/city to get weather data for that specific location.

- Upon launching the application, the current weather data will be displayed based on the user's current location (if granted permission).
- Alternatively, users can manually enter a location/city to fetch weather data for that location.
- To refresh weather data, simply press the  on the screen or tap the refresh button.


## API Reference
https://openweathermap.org/current

#### Using Latitude & Longitude 
```http
https://api.openweathermap.org/data/2.5/weather?lat={lat}&lon={lon}&appid={API_Key}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `{lat}` | `string` | **Required**, Latitude coordinate of current location |
| `{lon}` | `string` | **Required**, Longitude coordinate of current location|
| `{API_Key}` | `string` | **Required**, Your unique API key (you can always find it on your account page under the "API key" tab) |

#### Using City

```http
https://api.openweathermap.org/data/2.5/weather?q={City_Name}&appid={API_Key}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `{City_Name}` | `string` | **Required**, City |
| `{API_Key}` | `string` | **Required**, Your unique API key (you can always find it on your account page under the "API key" tab) |

#### Using Zip Code

```http
https://api.openweathermap.org/data/2.5/weather?zip={Zip_Code}&appid={API_Key}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `{Zip_Code}` | `string` | **Required**, Zip code of area |
| `{API_Key}` | `string` | **Required**, Your unique API key (you can always find it on your account page under the "API key" tab) |

## Application Demo Gif

https://github.com/mafaqcs/WeatherWithSwiftUI/blob/main/WeatherDemo.gif
