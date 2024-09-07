# GPS Locator using Python

This Python program retrieves your current geographical coordinates (latitude and longitude) based on your IP address and creates a visual map using the `folium` library. The map is saved as an HTML file and displayed in your browser.

## Features

- Retrieves location coordinates (latitude and longitude) using your IP address.
- Displays the current location on an interactive map.
- Saves the map as an HTML file.
- Opens the map in a web browser using Selenium.

## Prerequisites

Ensure that the following Python packages are installed:

- `requests`: For making HTTP requests to retrieve your IP information.
- `selenium`: For automating browser interactions.
- `folium`: For creating maps with your location data.
- Webdriver (Chrome): Required for Selenium to open the HTML file in a browser.

You can install these dependencies using the following command:

```
pip install requests selenium folium
```

Also, download the Chrome WebDriver from [here](https://sites.google.com/a/chromium.org/chromedriver/downloads) and ensure it is accessible in your system's PATH.

## How to Use

1. Clone this repository or download the source code.
2. Ensure you have the required dependencies installed.
3. Run the program using Python:

```
python gps_locator.py
```

4. The program will:
   - Fetch your current geographical location.
   - Create an interactive map displaying your location.
   - Save the map as an HTML file with the current date as the file name.
   - Automatically open the map in your web browser.

5. The map will close after 10 seconds, and the program will exit.

## How it Works

- **`locationCoordinates()`**: Fetches your IP address and retrieves location data from an external API (`ipinfo.io`).
- **`gps_locator()`**: Creates an HTML file using `folium` to show your location on a map, saves it, and returns the file name.
- **Main Function**: Uses Selenium to open the HTML file in your default browser, displays the map for 10 seconds, and then closes the browser.

## Troubleshooting

- If the browser does not open, ensure that you have downloaded the correct version of Chrome WebDriver.
- If you encounter issues with the map not being displayed, verify your internet connection as the program relies on online APIs for location data.

## License

This project is licensed under the MIT License.
```
