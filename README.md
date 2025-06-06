# SmartThermostat
Smart thermostat project using Azure Sphere MT3620 and Raspberry Pi. Monitors temperature, humidity, and motion; automates furnace via schedules and predictions.
# Contents
- Smart_Thermostat_Report.pdf: Project report detailing the smart thermostat system.
- LICENSE: Creative Commons Attribution 4.0 International License.
# Project Details
Developed for the IoT-2 course (CSE210) at Sri Ramachandra Institute of Higher Education and Research, this project implements a smart thermostat using the Azure Sphere MT3620 and Raspberry Pi B+. Key features:
- Configurable Schedules: Set daily heating cycles with adjustable durations.
- Motion Detection: Uses a PIR sensor to activate/deactivate the display and switch to a baseline temperature mode after prolonged inactivity (1–6 days).
- Web Interface: Hosted on Raspberry Pi, allows remote temperature adjustments and schedule configuration.
- Data Logging and Visualization: Stores sensor data (temperature, humidity) in InfluxDB and visualizes via Grafana.
- Predictive Model: Estimates indoor temperature and furnace runtime using local weather data and UV index, with accuracy within 5–20 minutes.

# Hardware
- Azure Sphere MT3620 Starter Kit
- Raspberry Pi B+
- 0.96" OLED 64x128 Display Module
- Texas Instruments HDC1080 Humidity and Temperature Sensor
- PIR Sensor (7m range)
- Rotary Encoder with Push-Button
- Grove Solid State Relay V2
# Software
- Microsoft Azure for cloud integration
- InfluxDB for data storage
- Grafana for visualization
# Implementation
- Controls heating (no AC or fan, per hardware constraints).
- Integrates with smart home platforms (e.g., Alexa, Google Assistant).
- Uses geofencing for occupancy-based temperature adjustments.
- Optimizes energy use by learning user preferences and external conditions.
# How to Use
- Download Smart_Thermostat_Report.pdf and open in a PDF viewer (e.g., Adobe Acrobat, Google Chrome).
- Review the report for details on implementation, hardware, and software.
- To replicate the project:
  - Assemble the listed hardware components.
  - Configure the Azure Sphere MT3620 and Raspberry Pi with Microsoft Azure, InfluxDB, and Grafana.
  - Follow the report’s implementation section for setup and configuration.
# License
This project is licensed under the Creative Commons Attribution 4.0 International License. You are free to share and adapt the material, provided you give credit to the authors.
# Notes
- The PDF references output dates (Sept 26–29, 2023) but lacks specific output data. Include additional files (e.g., graphs, code) in the repository if available.
- The predictive model’s accuracy depends on occupancy and visitor patterns, which may require further tuning.

