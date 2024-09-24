# Smart IV Bag Monitoring System

## Overview

The Smart IV Bag Monitoring System is an IoT-based solution designed to automate the monitoring of intravenous (IV) fluid levels in healthcare facilities. By leveraging MQTT (Message Queuing Telemetry Transport) and WebSocket technologies, this system provides real-time updates on IV bag fluid levels, enhancing patient safety and operational efficiency.

## Technologies Used

- **MQTT**: For lightweight messaging between devices and the server.
- **ESP32**: A microcontroller that measures the IV bag weight and publishes data to an MQTT broker.
- **Node.js**: Acts as a bridge between the MQTT broker and the web application, handling subscriptions and WebSocket communication.
- **WebSocket**: For real-time communication between the Node.js server and the web application.
- **Bootstrap**: For styling the web application.
- **HX711**: Load cell amplifier for measuring weight.
- **Adafruit BMP280**: Barometric pressure sensor (if used for additional features).

## Project Setup

### Prerequisites

- **Node.js** and **npm**: Make sure you have Node.js and npm installed. You can download them from [nodejs.org](https://nodejs.org/).
- **MQTT Broker**: You can use Mosquitto or any other MQTT broker of your choice.
- **ESP32**: Ensure that your ESP32 development environment is set up. This includes the necessary libraries and tools for uploading code to the ESP32.

### Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/yourusername/iv-bag-monitoring.git
   cd iv-bag-monitoring
