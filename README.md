# M5Stack-Atom-esp32-pico-server-client-link
AM2305 data transmission using Wi-Fi
1. The ESP32 pico server creates its own wireless network (ESP32 Soft-Access Point). So, other Wi-Fi devices can connect to that network (SSID: ESP32-Access-Point, Password: 123456789).
2. The ESP32 pico client is set as a station. So, it can connect to the ESP32 server wireless network.
3. The client can make HTTP GET requests to the server to request sensor data or any other information. It just needs to use the IP address of the server to make a request on a certain route: /temperature, /humidity or /pressure.
4. The server listens for incoming requests and sends an appropriate response with the readings.
