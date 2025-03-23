Bistream or Binary Sequence
- a sequence by sending a high or low state rapidly a number of times
In order to interpret the data from the signals, we use [Serial Communication Protocols](https://docs.arduino.cc/learn/starting-guide/getting-started-arduino/#serial-communication-protocols).

Serial Communication Protocols
- used in order to interpret the data from the signals
- Most Common
	- UART
		- used to send data between a computer and arduino board
		- Example: uploading a new program
		- reading data directly from an android
	- SPI
		- communicate between both internal and external components
		- communication is handled by something called serial bus
	- I2C
		- communicate between both internal and external components
		- communication is handled by something called serial bus
		- we can connect several sensors on the same pin, and retrieve the data accurately

What are Sensors
- is used to _sense_ its environment, meaning it records a physical parameter, for example temperature, and converts it into an electronic signal.
- Button is also a sensor
- analog sensor is the easiest way to record data from a sensor
	- through altering the volatege input fed into and arduino analog pin
- Digital sensors are a bit more advanced
	- Digital Sensors rely on Serial Communication Protocols

Actuators
- used to actuate or change a physical state
- examples:
	- LED
	- Motor
	- Switch
- Actuators converts electric signals into radiant energy or mechanical energy
- How to control actuators
```c
digitalWrite(LED, HIGH);
digitalWrite(LED, LOW);

analogWrite(motor, 255);
analogWrite(motor, 25);
```


Input & Output
- Sensors and actuators are referred to as input and outputs
- it is common to construct conditionals that checks the state of a sensor and decides wheter its should actuate something

Using Libraries
`sensorValue = senosr.read();`


Memory:
- Arduino has two memories:
	- SRAM
		- store the value of a variable
		- on powered off this memory resets
	- Flash memory
		- used to store main program, or the instructions for the microcontroller
		- memory is not erased on powered off
	- 

# SENSORS:
### ANALOG
-  Mostly are 3 pins
- 1 pin is the ground
- 1 pin 5v input
- 1 pin reading output
- S stands for sensor and is our data output
- - means ground 
- the remaning pin is the 5v input
# Programming
Minimum requirement 
- `void setup()`
	- executes only once
	- used to initialize variables 
- `void loop()`
	- code we want to execute over and over again

Sketch
- Program in an Arduino Project
- is a file that you write your program inside
- `.ino` extension, always stored in a folder of the same name
- folder can include other files such as a header file


Common Functions
`delay()`
- pauses the program for a set number of milliseconds
- for efficiency of the code , its best to use `millis()`

`millis()`
- allow you to have multiple events happening simultaneously, without pausing the program

### Serial Communication
`Serial.begin()`
- initialize serial communication between board and computer
- defined in the board setup() function
`Serial.print()`
- prints data to the serial port

`Serial.read()`
- reads incoming serial data

### GPIO / Pin Management
`pinMode()`
- configures digital pin to behave as an input or output
- configured inside of the void setup()

`digitalRead()`
- reads the state of a digital pin

`digitalWrite()`
- Writes high or low state to a digital pin

`analogRead()`
- reads the voldate of an analog pin
- returns a value between 0-1023

`analogWrite()`
- writes a value between 0-255
- used for dimming lights, setting speed of motor
- also referred as PWM


# Questions:
What are noise,how does it come