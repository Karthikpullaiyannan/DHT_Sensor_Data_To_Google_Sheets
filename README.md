# 🌡️💧 DHT Sensor Data to Google Sheets

This project demonstrates how to use a DHT sensor to collect temperature and humidity data and send it to Google Sheets using an ESP8266/ESP32 microcontroller.

## Requirements

- DHT sensor (DHT11, DHT22, etc.)
- ESP8266 or ESP32 microcontroller
- Arduino IDE
- Google account

## Dependencies
-DHT Sensor Library
-ESP8266WiFi Library
-WiFiClientsecure Library

## Setting Up

1. Install the necessary libraries using the Arduino Library Manager.
2. Clone or download this repository.
3. Open the "DHT_Sensor_to_Google_Sheets.ino" file in the Arduino IDE.
4. Update the following variables in the code:
   - 'WIFI_SSID': Your WiFi network SSID.
   - 'WIFI_PASSWORD': Your WiFi network password.
   - 'SHEET_ID`: ID of your Google Sheets document.
   - 'SHEET_NAME': Name of the worksheet where you want to store the data.
   - 'DHT_PIN': The pin to which your DHT sensor is connected.
5. Upload the code to your ESP8266/ESP32 board.
6. Open the serial monitor to view the IP address of your ESP8266/ESP32.
7. Open the Google Sheets document and verify that the temperature and humidity data are being sent.

## Google Sheets Setup

1. Create a new Google Sheets document.
2. Rename the first sheet to 'Data'.
3. In the first row, add the following headers: 'Timestamp', 'Temperature (°C)', 'Humidity (%)'.
4. Share the document with the email address obtained from the Google Cloud Platform.
5. Retrieve the 'SHEET_ID' from the URL of your Google Sheets document.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
