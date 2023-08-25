# Smart-Wheelchair-for-Quadriplegic-Patients


# Abstract 
The health service sector has been continuously trying to prove and improve the service given to the Quadriplegic Patients in need of mobility
assistance. As a result, more Efforts have been directed towards development of smart wheelchairs. This project aims to design a wheelchair which
is controlled by a wireless connected Smartphone via Voice which replicates
the commands given by the patients through a secure dedicated Web server
to the wheelchair. The patients will be able to move their wheelchairs forward, back, right or left at a designated speed. The Wheelchair would be
employed with various health monitoring systems such as ECG, Heart rate,
Pulse, etc. All the health related information collected from these sensors
would be displayed on a website accessible for doctors and patient’s relatives. It would also have state-of-the-art safety features facilitated by
proximity sensor, Gyroscopic sensor, IR Line following sensor and a safety
latch. A Gimbal mechanism would also be added to ensure a stabilized leveled movement of the wheelchair over an uneven path. Arduino uno will
act as the brain as it will control the movement and gather information
from various sensors. 

# Limitations of existing system 
Several researchers have proposed various innovative systems for wheelchair
control. Prof. Rajesh Kannan has proposed a camera-based system that
tracks finger movements to control the direction of the wheelchair. Aleksandar Pajkanovic and Branko Dokic have designed a robotic wheelchair that
can be controlled using head gestures, which are detected by an accelerometer and a microcontroller. Sobia M. Carmel has developed a facial recognition system that enables the user to control the wheelchair using face
detection, facial expression recognition, and command generation. Klabi
has illustrated the use of voice commands and facial movements to control
the wheelchair, along with sensors for obstacle detection and avoidance.
Lastly, Andrej Skraba has presented a cloud-based wheelchair platform ˇ
that can be controlled through speech using a low-cost WebKit. We have
implemented several innovative and new features in addition to the previously researched voice control mechanism. The biggest novelty being
application of Mecanum wheels for increased mobility. In order to ensure
Patient’s utmost comfort we also have executed and fine]-tuned a gimbal
stabilization to the wheelchair. An additional modernization also being
the implementation of IOT to the wheelchair, which shares vital medical
statistics of the patient to the concerned authorities via a secure network
and server. 
# Problem Statement 
To Develop a wheelchair for quadriplegics patients who are unable to use
their arms and legs due to Quadriplegia, track their medical statistics with
the help of sensors, and provide a comfortable ride with the help of a
self-stabilizing gimbal. 

# Solution 
Our system’s main goal is to provide freedom of mobility to the Quadriplegic
patients and the other patients in need. Our initiative aims to help patients
overcome their disability and contribute to the medical profession.
• Monitoring the health of patients: Health sensors can be used to keep
an eye on patients’ wellbeing. which can help doctors determine the
appropriate course of action.
• Multiple Sensors: We use several sensors to gather all the information
required, receive vocal orders from the patient, and carry out the task.
• Mobility and Stability: The movement mechanism is equipped with a
mechanum wheel and gimbal for the patients’ safety. All-directional
movement is provided by the mechanical wheel, while three-axis stability is provided by the gimbal’s usage of gyro sensors. 

# 3D Model 
The following images gives us a idea about the realworld implementation
of wheelchair . the mecanum wheels as seen in the images improves the
mobility of the wheelchair by providing side ways , diagonal, rotating and
froward-backward motion. the quadriplegic patient will sit on the chair
which is stabilised with the help of a gyro sensor and servo motors to keep
the chair level at all times.

![image](https://github.com/mansiawachat/Smart-Wheelchair-for-Quadriplegic-Patients/assets/72509388/eb15dea1-1fe5-46d5-a2dd-8e9f700fc1a5) 
![image](https://github.com/mansiawachat/Smart-Wheelchair-for-Quadriplegic-Patients/assets/72509388/b326e986-8ad0-49f7-936c-835a7e81d964)
![image](https://github.com/mansiawachat/Smart-Wheelchair-for-Quadriplegic-Patients/assets/72509388/6e2ceabb-a701-4ccb-98fb-06ae15b6ffe4)

# Stabilizing Module 
In the project lab, the stabilizing module was designed in Autodesk Fusion
360 and 3-D printed.Because of its high density, strength and resistance to
wear and tear, we chose PLA filament.The stabilizing module was designed
with the components that will be placed inside it in mind. It also holds
the health monitoring systems and stabilizing mechanism
![image](https://github.com/mansiawachat/Smart-Wheelchair-for-Quadriplegic-Patients/assets/72509388/041ad42e-4d0b-40c3-9c0a-094a0f610af4)
![image](https://github.com/mansiawachat/Smart-Wheelchair-for-Quadriplegic-Patients/assets/72509388/ec80c718-99d1-4c72-b0ed-c2ae12b6e432)
![image](https://github.com/mansiawachat/Smart-Wheelchair-for-Quadriplegic-Patients/assets/72509388/101a6ee6-ac5f-4f49-bc3a-be9c6e2457cf)
![image](https://github.com/mansiawachat/Smart-Wheelchair-for-Quadriplegic-Patients/assets/72509388/89115e9e-855c-4e54-8240-f248843bd308)
# Block Diagram 

![image](https://github.com/mansiawachat/Smart-Wheelchair-for-Quadriplegic-Patients/assets/72509388/9ae35852-78c6-4232-b7f5-d4e1a920ffa9)

The Arduino of the stabilization module takes input from the heart
rate, O2 sensor, and EEG sensor simultaneously, to broadcast it over a
secure website. The same Arduino then accepts input from the gyro sensor,
which in turn commands the Servo Motors to provide an active stabilization
process. The second Arduino of the mobility module accepts inputs from
the IR sensor, proximity sensor, and Bluetooth module simultaneously to
instruct the stepper driver which powers the stepper motor thus operating
the Mecanum wheels in the patient’s desired direction. 

![image](https://github.com/mansiawachat/Smart-Wheelchair-for-Quadriplegic-Patients/assets/72509388/c0e085bd-6f4b-40ae-b322-d3c16c343d41) 

The circuit is powered on and all the sensors data is fetched by sql and
used by xampp to post the collected data on the website. simultaneously
the arduino checcks for given voice commands and depending upon the
free space availbale the wheelchair moves in the that direction and the
stabilizing of the patient is provided by gimabl which uses gyroscope to
maintian the patients level. 

![image](https://github.com/mansiawachat/Smart-Wheelchair-for-Quadriplegic-Patients/assets/72509388/2d0db846-f0eb-40a2-959d-8254df7b687c)

# Hardware Implementation 
The quadriplegic patient is set up in the wheelchair, they control the movement and direction with the help of their voice commands namely Left,
Right, Forward, Back, and Stop. The Wheelchair has three types of sensors
for different operations namely mobility, stabilization, and health monitoring. The Bluetooth sensor, proximity sensor, and IR sensor give inputs
to the Arduino which controls the locomotion. The O2 sensor, ECGsensor, and heart rate sensor monitor the patient’s health statistics. The
Arduino controls stepper motor drivers which are connected to Mecanum
wheels. These wheels offer more mobility and flexibility in maneuvering
the wheelchair. The wheelchair stabilization module consists of three Servo
Motors which actively keep the patient settled and leveled over rough terrain. The wheelchairs data such as patient’s stats and live location is
broadcasted on a secure website which can be accessed by the patient’s
doctor and relatives for added convenience. The wheelchair helps to make
the patient’s life more convenient and happy.  


![image](https://github.com/mansiawachat/Smart-Wheelchair-for-Quadriplegic-Patients/assets/72509388/21477deb-b949-4059-a27f-82a2ceeeaa44)

![image](https://github.com/mansiawachat/Smart-Wheelchair-for-Quadriplegic-Patients/assets/72509388/93d90d29-e6d9-4765-9827-f35006375145) 

# Sensor Readings 

![image](https://github.com/mansiawachat/Smart-Wheelchair-for-Quadriplegic-Patients/assets/72509388/0b68771e-8c2e-40aa-a7ae-7153c5fd7adc)

The blynk IoT cloud provides features for web dashboards as well as
mobile dashboards, These dashboards allows us to display, analyze and
visualize the required outcome from the readings taken from sensors.along
with this blynk can also monitor and maintain the database along with
live data. 

# Future scope 
Here are some areas where the wheelchair can developed further by enhancing and adding additional features.

1. A safety lock system can be added in the wheelchair where in the
wheelchair only works when the seat belt is latched properly

2. Additional functionality to the Gyroscope sensor can be added to measure the incline and alert the patient and decrease speed of the wheelchair
in case of a slope.

3.With the help of IR sensor we can develop a blink sensor which controls the acceleration, speed settings and braking of the wheelchair.

4. We can further use IR sensors as a line follower mechanism so the
wheelchair may move without any constant input from the patient.

6. Sip and Puff system, based on concept of air pressure to control the
movement of the wheelchair.

7. Solar charged battery for increased efficiency and sustainability.

