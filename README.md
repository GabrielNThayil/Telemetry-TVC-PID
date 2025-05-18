# MPU6050 Servo Gimbal with PID Control #

This project demonstrates a basic gimbal-like setup using the MPU6050 accelerometer/gyroscope module and a servo motor. 
The pitch angle of the device is calculated in real-time and used to control a servo using a PID controller. Additionally, temperature and humidity data are logged from a DHT22 sensor.

# Components Used # 
1) Arduino UNO (Wokwi-compatible)
2) MPU6050 Accelerometer + Gyroscope
3) DHT22 Temperature and Humidity Sensor
4) Servo Motor (eg. SG90)
 Optional: Wokwi simulation setup

# Features #
Real-time pitch calculation using MPU6050
Servo angle mapped from pitch data
PID control loop to stabilize motion
DHT22 temperature & humidity readings
JSON-style serial output for telemetry/logging

# Project Output #

The system prints data over Serial in this format:

json
{
  "temp": 24.0,
  "humidity": 58.9,
  "pitch": 12.73,
  "servo": 114
}
Raw acceleration data is also shown for debugging:
ax: -0.35, ay: 1.33, az = 9.81 
