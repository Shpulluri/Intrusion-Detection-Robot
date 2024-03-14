# GUARDZILLA - Intrusion-Detection-Robot
### Overview:
This project implements an Intrusion Detection Robot using Raspberry Pi, OpenCV for image processing, and Flask for web server functionality. The robot is designed to detect intruders through a live camera feed, trigger an alarm, capture an image of the intruder, and send an email notification to the user.

### Features:
- Live Video Feed: The robot provides a live video feed accessible via a web browser, allowing remote monitoring of the area.
- Intruder Detection: Utilizes OpenCV's Haar Cascade Classifier to detect faces in the video feed, identifying potential intruders.
- Alarm Activation: Upon detecting an intruder, the robot triggers a buzzer alarm to alert the user.
- Email Notification: Sends an email notification with an attached image of the intruder to the user's email address.
- Remote Control: Allows remote control of the robot's movement via a web interface.
  ![image](https://github.com/Shpulluri/Intrusion-Detection-Robot/assets/93041504/bad32de8-8239-451c-bd06-9a20e56bf777)


  ### Components:
- Raspberry Pi: Acts as the central processing unit, responsible for image processing, email sending, and web server hosting.
- Camera Module: Captures the live video feed for intruder detection.
- Buzzer: Used to trigger an alarm upon intrusion detection.
- Python Libraries: Utilizes libraries such as OpenCV, Flask, GPIOZero, and smtplib for image processing, web server hosting, GPIO control, and email sending, respectively.

  ### Hardware Setup:
- Install the Raspberry Pi OS on an SD card following the official Raspberry Pi documentation.  
- Connect the camera module to the Raspberry Pi's camera port. Ensure it's properly seated and secured.
- Enable the camera interface in the Raspberry Pi configuration settings using the raspi-config tool.
- Connect the buzzer to the GPIO pins of the Raspberry Pi. Ensure you've identified the correct GPIO pins for input/output and power.
- If your robot includes motor and wheel setup for movement control:
- Connect the motors to the GPIO pins using a motor driver board and securely attach the wheels to the motor shafts.
  
### Software Setup:
- Python Environment:
  Ensure Python is installed on your Raspberry Pi. You can check by running python --version in the terminal.
  Install necessary Python libraries using pip install opencv-python flask gpiozero.
  
- Code Configuration:
  Modify the code to include your email address, email server settings, and any other required configurations.
  Ensure the GPIO pin numbers in the code match your hardware setup.
  
- Web Server Configuration:
  Configure the Flask web server to run on your Raspberry Pi. Set the appropriate host and port in the Flask app.
