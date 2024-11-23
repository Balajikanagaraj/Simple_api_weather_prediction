# Weather App

## **Overview**
The Weather App is a simple web application designed to display the current weather conditions for a specific location (Coimbatore in this case). It fetches real-time weather data using the OpenWeatherMap API and dynamically updates the webpage with details like temperature, weather description, and an icon representing the weather.

---

## **Features**
- Displays the current weather conditions:
  - **Location name**
  - **Temperature in Celsius**
  - **Weather description** (e.g., sunny, cloudy, rainy)
  - **Weather icon** representing the current conditions
- **Refresh button** to reload and fetch the latest weather data.
- Clean and responsive user interface.

---

## **Technologies Used**
- **HTML5**: Webpage structure
- **CSS3**: Styling and layout
- **JavaScript**: Dynamic data fetching and DOM manipulation
- **OpenWeatherMap API**: Source of weather data
- **Font Awesome**: Icons for styling
- **Google Fonts**: Typography (Poppins font)

---

## **How It Works**
1. The app sends an AJAX request to the OpenWeatherMap API.
2. Parses the API response to extract relevant data:
   - **Weather description:** e.g., "clear sky"
   - **City name:** e.g., "Coimbatore"
   - **Temperature:** Converts from Kelvin to Celsius
   - **Weather icon URL**
3. Updates the webpage dynamically with this data.
4. The refresh button reloads the page for updated weather.

---

## **Setup and Installation**
1. Clone or download the repository.
2. Obtain an API key from [OpenWeatherMap](https://openweathermap.org/api).
3. Replace the `appid` parameter in the API URL with your key:
   ```javascript
   var link = "https://api.openweathermap.org/data/2.5/weather?q=coimbatore&appid=YOUR_API_KEY";
