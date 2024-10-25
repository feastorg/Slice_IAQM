## IAQM - Industrial Air Quality Monitor 

## Requirements

### Requirements List

- **Data Logging**
  - Logging of data to SD card
  - Real-time clock for accurate data logging

- **Feedback Alarms**
  - Visual feedback alarm
  - Auditory feedback alarm

- **Air Quality Readings**
  - Ambient temperature sensor
  - Ambient humidity sensor
  - Barometric pressure sensor
  - CO gas sensor
  - CH₄ gas sensor
  - NH₃ gas sensor
  - H₂S gas sensor
  - H₂ gas sensor
  - Smoke / flammable gas sensor
  - VOCs (Volatile Organic Compounds)
    - eCO2 readings
  - AQI (Air Quality Index)

### Component Table

| **Name**            | **Parameters Measured**                                         | **Value Abbreviation** | **Notes**                                                                                  |
|---------------------|-----------------------------------------------------------------|------------------------|-------------------------------------------------------------------------------------------|
| SD Card Reader      | Data Logging                                                    | N/A                    |                                                                                           |
| Real Time Clock     | Global Local Time                                               | N/A                    |                                                                                           |
| Piezo Buzzer        | Auditory Feedback                                               | N/A                    | For Alarm                                                                                      |
| Large LED           | Visual Feedback                                                 | N/A                    | For Alarm                                                                            |
| MQ-7                | Carbon Monoxide                                                 | CO                     | 10～500ppm, needs cycled coil heating.                                                                                |
| MQ-137              | Ammonia Gas                                                     | NH₃                    | 5～500ppm                                                                                  |
| MQ-8                | Hydrogen Gas                                                    | H₂                     | 100～1000ppm                                                                               |
| MQ-136              | Hydrogen Sulfide Gas                                            | H₂S                    | 1～200ppm                                                                                  |
| MQ-2                | Smoke / Combustible Gas                                          | N/A                    | 300～10000ppm (flammable gas)                                                             |
| MQ-3                | Alcohol Gas                                                     | C₂H₅OH                 | 25 ~ 500ppm (alcohol). Detects alcohol gases like a breathalyzer, not added in default build. |
| MQ-4                | Methane CNG Gas                                                 | CH₄                    | 300～10000ppm                                                                              |
| MQ-6                | Liquefied Petroleum Gas (LPG)                                   | C₃H₈                   | 300～10000ppm (propane). Not in default build.                                                                    |
| BME 280             | Ambient Temperature, Relative Humidity, Barometric Pressure     | N/A                    | Ambient Temp. -40 - +85 °C, Rel. Humidity 0 - 100 %, Baro. Pressure 300 - 1100 hPa                                 |
| ENS160              | Total Volatile Organic Compounds, Equivalent Carbon Dioxide, Air Quality Index | TVOC, eCO₂, AQI        | TVOC 0 – 65,000 ppb, eCO2 400 – 65,000ppm (CO₂ equiv.), AQI-UBA 1 to 5 |

### PV Box

| **Name**            | **Parameters Measured**                                         | **Value Abbreviation** | **Notes**                                                                                  |
|---------------------|-----------------------------------------------------------------|------------------------|-------------------------------------------------------------------------------------------|
| SD Card Reader      | Data Logging                                                    | N/A                    |                                                                                           |
| Real Time Clock     | Global Local Time                                               | N/A                    |                                                                                           |
| Piezo Buzzer        | Auditory Feedback                                               | N/A                    | For Alarm                                                                                      |
| Large LED           | Visual Feedback                                                 | N/A                    | For Alarm                                                                            |
| MQ-7                | Carbon Monoxide                                                 | CO                     | 10～500ppm, needs cycled coil heating.                                                                                |
| MQ-137              | Ammonia Gas                                                     | NH₃                    | 5～500ppm                                                                                  |
| MQ-8                | Hydrogen Gas                                                    | H₂                     | 100～1000ppm                                                                               |
| MQ-136              | Hydrogen Sulfide Gas                                            | H₂S                    | 1～200ppm                                                                                  |
| MQ-4                | Methane CNG Gas                                                 | CH₄                    | 300～10000ppm                                                                              |
| MQ-9B                | Carbon Monoxide & Methane CNG Gas                                                 | CO & CH₄                    | 10～500ppm CO, 300～10000ppm CH4                                                                              |
| BME 280             | Ambient Temperature, Relative Humidity, Barometric Pressure     | N/A                    | Ambient Temp. -40 - +85 °C, Rel. Humidity 0 - 100 %, Baro. Pressure 300 - 1100 hPa                                 |
| ENS160              | Total Volatile Organic Compounds, Equivalent Carbon Dioxide, Air Quality Index | TVOC, eCO₂, AQI        | TVOC 0 – 65,000 ppb, eCO2 400 – 65,000ppm (CO₂ equiv.), AQI-UBA 1 to 5 |

### Parts List

- SD conn: https://www.mouser.ca/ProductDetail/Molex/502570-0893?qs=xbccQsLEe0eiL%252BVgS3E4nA%3D%3D
- SD level shifter: https://www.mouser.ca/ProductDetail/Texas-Instruments/TXB0104D?qs=oFXvjAmG9Eh0u9dpGkn5zg%3D%3D
- batt holder: https://www.mouser.ca/ProductDetail/Keystone-Electronics/3000?qs=Mn60vILZNNbcLh3ZnzbtUw%3D%3D