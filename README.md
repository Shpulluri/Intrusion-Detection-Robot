# Intrusion-Detection-Robot
### Overview:
This project implements an Intrusion Detection Robot using Raspberry Pi, OpenCV for image processing, and Flask for web server functionality. The robot is designed to detect intruders through a live camera feed, trigger an alarm, capture an image of the intruder, and send an email notification to the user.

### Features:
- Live Video Feed: The robot provides a live video feed accessible via a web browser, allowing remote monitoring of the area.
- Intruder Detection: Utilizes OpenCV's Haar Cascade Classifier to detect faces in the video feed, identifying potential intruders.
- Alarm Activation: Upon detecting an intruder, the robot triggers a buzzer alarm to alert the user.
- Email Notification: Sends an email notification with an attached image of the intruder to the user's email address.
- Remote Control: Allows remote control of the robot's movement via a web interface.

  ### Components:
- Raspberry Pi: Acts as the central processing unit, responsible for image processing, email sending, and web server hosting.
- Camera Module: Captures the live video feed for intruder detection.
- Buzzer: Used to trigger an alarm upon intrusion detection.
- Python Libraries: Utilizes libraries such as OpenCV, Flask, GPIOZero, and smtplib for image processing, web server hosting, GPIO control, and email sending, respectively.
