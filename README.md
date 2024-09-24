# Adaptive Cruise Braking System 

This project is a prototype of an **Adaptive Cruise Braking System**, developed using an Arduino, ultrasonic and IR sensors. The system detects obstacles in front of a vehicle and automatically applies brakes if an object is detected within a certain distance. This prototype mimics the functionality of modern autonomous braking systems found in vehicles.

## Features
- **Obstacle Detection**: Utilizes both ultrasonic and IR sensors to detect objects in front of the vehicle.
- **Autonomous Braking**: Automatically stops and reverses the vehicle when an obstacle is detected within a threshold distance.
- **Servo-Controlled Scanning**: A servo motor moves the ultrasonic sensor to scan both left and right to decide the safest turn direction.
- **Adaptive Movement**: Based on obstacle distance, the system adjusts the motor speed and direction for smooth turning and navigation.

## Components Used
- **Arduino UNO/Nano**: The microcontroller to run the code.
- **Ultrasonic Sensor (HC-SR04)**: Used for distance measurement in front of the vehicle.
- **IR Sensor**: For additional object detection capability (can be optional based on your setup).
- **Adafruit Motor Shield**: Controls 4 DC motors (2 for forward/backward movement and 2 for turning).
- **DC Motors**: Four motors control the movement of the vehicle.
- **Servo Motor**: Rotates the ultrasonic sensor for side detection.
- **Battery Pack**: To power the motors and Arduino.

## How It Works
1. The ultrasonic sensor continuously measures the distance to the nearest object in front of the vehicle.
2. If the object is within a predefined range (15 cm), the system stops the vehicle, moves it backward slightly, and scans the surroundings.
3. The servo motor rotates the ultrasonic sensor left and right to determine the better side to turn.
4. Based on the distance readings, the system decides whether to turn left or right, and then resumes forward motion.
5. If no object is detected within the danger zone, the vehicle continues to move forward.
6. The system also adjusts the speed of the motors based on the distance, slowing down when obstacles are near and stopping if too close.
7. 

## Contribution
Feel free to submit issues or pull requests for improvements. Contributions are welcome!
