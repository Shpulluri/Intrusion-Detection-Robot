# GUARDZILLA - Intrusion-Detection-Robot
### Overview:
This project implements an Intrusion Detection Robot using Raspberry Pi, OpenCV for image processing, and Flask for web server functionality. The robot is designed to detect intruders through a live camera feed, trigger an alarm, capture an image of the intruder, and send an email notification to the user.

### Features:
- Live Video Feed: The robot provides a live video feed accessible via a web browser, allowing remote monitoring of the area.
- Intruder Detection: Utilizes OpenCV's Haar Cascade Classifier to detect faces in the video feed, identifying potential intruders.
- Alarm Activation: Upon detecting an intruder, the robot triggers a buzzer alarm to alert the user.
- Email Notification: Sends an email notification with an attached image of the intruder to the user's email address.
- Remote Control: Allows remote control of the robot's movement via a web interface.
  
  ![image](https://github.com/Shpulluri/Intrusion-Detection-Robot/assets/93041504/f9c7a4fd-94c5-4f58-a827-2db0c7360521)

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

  ![image](https://github.com/Shpulluri/Intrusion-Detection-Robot/assets/93041504/5306f477-e9e4-4ae5-a5bb-922efea12694)
  

### Software Setup:
- Python Environment:
  Ensure Python is installed on your Raspberry Pi. You can check by running python --version in the terminal.
  Install necessary Python libraries using pip install opencv-python flask gpiozero.
  
- Code Configuration:
  Modify the code to include your email address, email server settings, and any other required configurations.
  Ensure the GPIO pin numbers in the code match your hardware setup.
  
- Web Server Configuration:
  Configure the Flask web server to run on your Raspberry Pi. Set the appropriate host and port in the Flask app.


### Running the application:
- Clone the repository to your Raspberry Pi by running the following command in the terminal:
  'git clone https://github.com/Shpulluri/Intrusion-Detection-Robot/'

- Execute the following command to start the web server and intrusion detection functionality:
  'python integrate.py'
  'python move.py'
  'python intrusion_detection_robot.py'

- Once the application is running, open a web browser on any device connected to the same network as the Raspberry Pi.Enter the IP address of the Raspberry Pi followed by port 5000 in the address bar (e.g.,     
  http://<raspberry_pi_ip>:5000/). You should now be able to view the live video feed and control the robot remotely using the arrow buttons on the web interface.


