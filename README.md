## Weather Fetcher CLI App

### Overview
Weather Fetcher is a Python command-line application that allows users to fetch and display real-time weather information for a specified city. It utilizes a weather API (e.g., OpenWeatherMap) to retrieve weather data and provides options to save reports for future reference.

---

### Features
- Fetches current weather details for a given city.
- Displays:
  - Temperature (Celsius/Fahrenheit).
  - Humidity percentage.
  - Weather description (e.g., clear sky, light rain).
- Option to save the weather report to a file in TXT or JSON format.
- Provides clear error messages for invalid input or API issues.

### Requirements
- Python 3.7 or higher
- Dependencies:
- `requests` for API communication

---

### Installation
- Clone the repository:
```
git clone git@github.com:devkinoti/weather_app_cli.git
cd weather_app_cli
```

---

### Install dependencies:

### Configure the API key:

- Sign up at OpenWeatherMap (or your chosen API provider) to obtain an API key.
- Create a .env file in the project directory and add your API key:

```
API_KEY=your_api_key_here
```

### Usage
- Run the application from the command line:

- Fetch weather data for a city:

```
python main.py --city "City Name"
```

Example:

```
python main.py --city "London"
```

### Save the weather report to a file:

```
python main.py --city "City Name" --save --format txt

```

### Supported formats: txt, json

Display usage instructions:

```
python main.py --help
```

### Example Output

Console Output:

```
City: London
Temperature: 15°C (59°F)
Humidity: 65%
Weather: Clear sky
```

### Saved File (weather_london.txt):

```
Weather Report for London
-------------------------
Temperature: 15°C (59°F)
Humidity: 65%
Weather: Clear sky
```

### Error Handling
Displays an error message if the city is not found:
```
Error: City not found. Please check the city name and try again.
```

Handles API issues like invalid API key or rate limits:
```
Error: Unable to connect to the weather service. Please try again later.
```

### Future Enhancements
- Add support for fetching weather for multiple cities in a single command.
- Include a 7-day weather forecast option.
- Provide localization options for weather descriptions.

### Contribution
- Fork the repository.
- Create a feature branch:

```
git checkout -b feature-name
```

Commit your changes:
```
git commit -m "Description of changes"
```

Push the branch:
```
git push origin feature-name
```

Create a pull request.

---

### License
This project is licensed under the MIT License. See the LICENSE file for details.

Author
Chris Kinoti
