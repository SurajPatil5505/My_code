# BLE Beacon with ESP32 for Store Promotions  

##  **Project Overview**  
This project demonstrates the use of an ESP32 microcontroller as a BLE (Bluetooth Low Energy) beacon that broadcasts a URL. The URL can be received by nearby mobile phones with Bluetooth enabled. Upon opening the URL, users are redirected to a web page displaying information about your store, such as:  
- Sales offers  
- Discount offers  
- New arrivals  
- Other promotional content  

##  **Key Features**  
- **BLE Beacon Functionality**: The ESP32 acts as a BLE beacon, continuously transmitting a custom URL.  
- **URL Broadcasting**: The transmitted URL redirects users to a web server hosting the store's promotional information.  
- **User Engagement**: Nearby mobile devices detect the beacon and receive the URL via the phone's notification system (on compatible devices).  
- **Web Server Integration**: The web server provides real-time information about the store's offers and promotions.  

##  **Hardware Requirements**  
- ESP32 Development Board  
- Micro USB Cable  
- Power Source for the ESP32 (e.g., USB power adapter or battery pack)  
- Mobile phone with Bluetooth enabled  

##  **Software Requirements**  
- Arduino IDE (for programming the ESP32)  
- BLEPeripheral library or ESP32 BLE library  
- Access to a web server to host the promotional website  

##  **Project Workflow**  
### 1. **ESP32 BLE Beacon Setup**  
- The ESP32 is programmed to operate as a BLE beacon using the ESP32 BLE library.  
- A custom URL (e.g., `http://mystore.com/offers`) is set to broadcast via BLE.  
- The beacon transmits the URL at regular intervals.  

### 2. **Mobile Phone Detection**  
- Nearby Bluetooth-enabled mobile phones detect the BLE beacon.  
- The phone displays a notification with the broadcasted URL (if supported by the operating system).  

### 3. **Web Server Integration**  
- When the user clicks the URL, it opens in their mobile browser.  
- The web server hosts a store-specific landing page with the following features:  
  - Current sales and discounts  
  - New arrivals  
  - Store location and contact information  

### 4. **User Interaction**  
- Customers interact with the webpage to explore ongoing promotions and store offerings.  

