# Smart_Weather_Station

This project involves creating an ESP32-based smart weather station that is capable of monitoring and reporting key environmental parameters including temperature, humidity, and rain status. The core components of the system include:
ESP32 Microcontroller: This serves as the central processing unit of the weather station. It handles data collection from sensors, processes the data, and hosts a web server to make the information accessible over a network.

DHT11 Sensor: This sensor is used for measuring temperature and humidity. It provides digital output data which the ESP32 can easily read and process.
Rain Sensor: A digital rain sensor is used to detect the presence of rain. The sensor provides a high or low signal which indicates whether rain is detected or not.
Wi-Fi Connectivity: The ESP32 connects to a Wi-Fi network using specified SSID and password credentials. This enables the weather station to be accessible from any device on the same network.

Web Server Interface: The ESP32 hosts a web server on port 80. Through this server, users can access a web page that displays the current temperature, humidity, and rain status. The web page is designed with HTML, CSS, and JavaScript, and it refreshes data every 10 seconds to ensure up-to-date information.
Real-Time Data Updates: The system reads sensor data at regular intervals and updates the web interface accordingly. This provides users with near real-time monitoring of environmental conditions.
Serial Monitoring: For debugging and monitoring purposes, the ESP32 outputs sensor readings and connection status to the serial console.

Functional Details:
Temperature and Humidity Reading: The DHT11 sensor reads temperature and humidity every few seconds. If the sensor fails to read data, the system handles the error gracefully.
Rain Detection: The rain sensor detects rain and sends a signal to the ESP32, which then processes this information and updates the web interface.
Web Interface Design: The web interface is styled to be user-friendly and visually appealing. It uses icons to represent different weather parameters and displays data in a clear and concise manner.

Code Breakdown:
Initialization: The ESP32 initializes the sensors and connects to the Wi-Fi network. It then sets up the web server routes and starts the server.
Data Handling: Functions are defined to read temperature, humidity, and rain status from the respective sensors. These functions are called when the web server requests data.
Web Server Routes: The server routes are defined to serve the main web page and handle requests for temperature, humidity, and rain data.

This project effectively demonstrates the capabilities of the ESP32 in building an IoT-based weather monitoring system. It combines hardware and software components to provide a reliable and user-friendly solution for real-time weather tracking.





