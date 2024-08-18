# Surfs Up in LA

This app displays up-to-date surf conditions for beaches along the Los Angeles coastline. Users can select from seven tracked beach locations, each displaying relevant surf and weather data in a simplified, user-friendly layout. 

## Features

### User Experience
- **Beach Selection**: Users can choose from a dropdown menu featuring popular surf spots like Zuma Beach, Santa Monica, and Huntington Beach. The app automatically displays the most recently selected beach on reload, thanks to local storage functionality.
- **Dynamic Data Display**: The app fetches and displays crucial surf conditions, such as water temperature, wind speed, swell direction, and more. These details are presented in a clear and accessible table format, making it easy for users to understand the current conditions.
- **Fun Integration**: A relevant gif, fetched from the Giphy API, accompanies the surf data to make the experience more engaging and entertaining.

### Functionality and Technical Implementation
- **Dropdown Menu and Local Storage**: The dropdown menu is designed with a default "Select beach" option to prevent accidental fetch requests. When a user selects a beach, its latitude and longitude are passed to the StormGlass API to retrieve the corresponding surf data. The app uses local storage to remember the user’s last selected beach and automatically display it on the next visit.
- **API Integration and Data Handling**: The app integrates with the StormGlass API to fetch necessary data, such as water temperature, air temperature, wind speed, and swell details. All fetched data is processed, including unit conversions (e.g., meters to feet, Celsius to Fahrenheit) and direction conversions (degrees to cardinal directions). The Giphy API is then called to fetch a gif that matches the surf conditions.
- **Algorithm and Data Processing**: An algorithm processes the surf data, determining the overall surf conditions, such as whether the waves are ideal for surfing or more challenging. This processed data informs the selection of the gif and the text displayed on the page.
- **Error Handling**: Robust error handling is implemented using JavaScript and JQuery. If a fetch error occurs (e.g., no available data), a modal popup alerts the user, ensuring a smooth user experience.

### What's the Future?


## Screenshots

![Mockup](https://github.com/shellienguyen/surf-forecast/blob/main/assets/images/surf-forecast1.jpg)
![Mockup](https://github.com/shellienguyen/surf-forecast/blob/main/assets/images/surf-forecast2.jpg)
