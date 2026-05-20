# BBloom - Cloud Based Plant Monitoring System

## Project Description
BBloom is a cloud-based plant monitoring system.
The system helps users monitor plant health using IoT sensors, image analysis, alerts and personalized recommendations.

The system allows users to:
- Monitor soil humidity, temperature, air humidity and light
- Upload plant images for AI analysis
- Detect diseases and pests
- Receive real-time alerts
- View plant health status in a dashboard
- Get recommendations for watering, fertilizing and treatment

## Architecture
The system is based on cloud architecture and Microservices.

Main components:
- Mobile Application
- IoT Sensors
- API Gateway
- Cloud Services
- Database
- Notification Service
- External Weather API

The API Gateway is the entry point to the cloud services.
Each service is responsible for a specific task.
The system also supports event-driven behavior, where sensor data or image upload can trigger cloud functions.

## Services

### Sensor Service
Receives data from IoT sensors, including soil humidity, temperature, air humidity and light.

### Image Analysis Service
Analyzes plant images and detects diseases or pests.

### Monitoring Service
Checks the current condition of the plant based on sensor data and image analysis.

### Alert Service
Creates alerts when a problem is detected, such as low humidity or suspected disease.

### Notification Service
Sends notifications to the user.

### Recommendation Service
Provides personalized recommendations for watering, fertilizing and treatment.

### User Service
Handles user login, registration and user data.

## Usage Examples

### Example 1 - Sensor Data
A sensor sends soil humidity data to the cloud.
If the humidity is too low, the system creates an alert and sends a notification to the user.

### Example 2 - Image Analysis
The user uploads a plant image.
The system analyzes the image and returns a possible disease detection with treatment recommendations.

### Example 3 - Dashboard
The user opens the dashboard and sees plant health status, sensor values, alerts and history.

## Tests (Examples)

| Test | Result | 
|---|---|
| User login | Passed |
| Sensor data received | Passed |
| Dashboard response time | Passed |
| Image upload | Passed |
| Alert creation | Passed |
| Notification sending | Passed |
| AND search | Passed |
| OR search | Passed |
| Ranking mechanism | Passed |

## KPI and SLA

### KPI
- Dashboard response time
- System availability
- Alert delivery time
- Sensor reliability
- Security

### SLA
- System availability: 99%
- Dashboard response time: up to 3 seconds
- Alert delivery time: up to 5 seconds
- Sensor failure detection after 15 minutes without data
- Secure communication using HTTPS/TLS