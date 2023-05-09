# IoT-based table cleanliness management system

### Introduction
The table cleaning machine offers various advantages over conventional cleaning methods in addition to its performance. It not only reduces personnel expenses and saves time, but it also offers a cleaner, more reliable cleaning experience. By automating the procedure, the machine lowers the possibility of human error and guarantees that the entire table surface has been thoroughly cleaned.
The Arduino, an open-source microcontroller that can be programmed to carry out a variety of tasks, is the logic of the device. The Arduino acts as the machine's brain by having the capacity to operate numerous sensors and motors.The ultrasonic sensor, which emits high-frequency sound waves that bounce off objects and return to the sensor, is one of the main sensors utilized in the device. The sensor can gauge the distance to an object and identify any messes on a tabletop by timing how long it takes for the waves to return.
When a mess is detected, the Arduino sends a signal to the servo motor, which moves the cleaning arm into position. Equipped with a cleaning  brush, the arm then proceeds to clean the surface of the table. Once the cleaning is complete, the arm returns to its original position and the sensor continues to scan the table for any remaining messes.

### Materials needed
* Arduino Uno board
* Ultrasonic sensor
* Servo motor
* Jumper wires
* Cleaning arm
* Cleaning brush
* Breadboard

### Operational process
Setting up the Arduino microcontroller is the first step.The Arduino IDE is used to programme the microcontroller board, which can be downloaded from the Arduino website.
Connect the Arduino board to the ultrasonic sensor next. The existence of any things on the table top is determined by the ultrasonic sensor. Attach the 5V and GND pins of the Arduino board to the relevant VCC and GND pins of the ultrasonic sensor. Attach the sensor's TRIG and ECHO pins to the digital pins 12 and 11, respectively, on the Arduino board.
The ultrasonic sensor must now be configured to recognise any things on the tabletop. The servo motor will begin cleaning when the Arduino signals the presence of an item. C is the programming language utilized by the Arduino IDE.The cleaning mechanism must be carried across the table using the servo motor, which needs to be programmed. The brush is being used as the cleaning tool. The servo motor will move the cleaning mechanism back and forth over the table surface when the Arduino provides a signal to it.
In the table cleaning device, we have used two servo motors, one of which is connected to an ultrasonic sensor and the other of which is integrated with the wiper that is used to clean the table. The servo that is connected to the ultrasonic sensor first rotates 180 degrees and detects if anyone is sitting on the table or not. If there is no one on the table, the second servo, which is integrated with the wiper brush that is used to clean the table, rotates 180 degrees with the help of the servo and cleans the table. This process continues in a loop.
The servo motor moves the cleaning arm back and forth, allowing the cleaning pad or brush to clean the surface of the table.
After the cleaning is complete, the servo motor moves the cleaning arm back to its initial position.
The ultrasonic sensor continues to scan the table surface for additional messes, and the process repeats if any additional messes are detected.
The cleaning machine can be turned off when cleaning is complete.
