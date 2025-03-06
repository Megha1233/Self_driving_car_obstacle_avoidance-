# Self_driving_car_obstacles_avoidance-
"Self-Driving Car: Obstacle Avoidance System"
A self-driving car with obstacle avoidance is a project that aims to create an autonomous vehicle capable of detecting and avoiding obstacles in its path. 

The system integrates sensors like ultrasonic sensors, or LIDAR to gather real-time data about the car's surroundings. Machine learning algorithms or conventional programming techniques process this sensor data to identify obstacles and determine the best course of action. 

This technology is essential in making autonomous vehicles safer and more efficient, especially in dynamic environments with unpredictable challenges. It's widely applicable in robotics, smart city projects, and even educational purposes for learning about AI and control systems.

Features of a self-driving car with obstacle avoidance:

1.Autonomous Movement – The car moves forward and detects obstacles in its way.
2.Obstacle Detection – Uses ultrasonic sensors or LiDAR to sense obstacles at different distances.
3.Path Correction – The car takes corrective actions (stop, turn left/right, or reverse) upon detecting an obstacle.
4.Motor Control – Four DC motors controlled via an H-bridge motor driver shield.
5.Real-Time Processing – Processes sensor data and controls motors using an Arduino microcontroller.

Hardware Components:

1. Arduino Uno – The brain of the system, processes sensor inputs and controls motors.
2. Motor Driver Shield (L298D or similar) – Controls the four DC motors.
3. Ultrasonic Sensor (HC-SR04) / LiDAR – Detects obstacles and measures distances.
4. Infrared Sensors (optional) – Used for close-range obstacle detection or line-following.
5. DC Motors (4x) – Drive the car's wheels.
6. Wheels & Chassis – Supports the movement of the vehicle.
7. Power Supply – A 9V battery for the motor driver and external power for Arduino.
   
Software Requirements:
Arduino IDE – To write and upload the code to Arduino.
Embedded C / C++ – Programming language for writing the control logic.

Libraries Used:
NewPing.h (for ultrasonic sensor)
AFMotor.h (for Adafruit Motor Shield)

Working Principle:

1. The car moves forward continuously.
2. The ultrasonic/LiDAR sensor detects obstacles ahead.
3. If an obstacle is within a defined range (e.g., <20 cm):
   The car stops.
   The system checks for a clear path on the left and right.
   It turns in the direction where there is more space.
   If no clear path is found, it reverses and retries.
4. Once a clear path is found, the car resumes forward movement.





