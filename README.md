# Temperature Based Fan Speed Control

INTRODUCTION
This circuit project is mainly used for varying the speed of a fan according to the temperature.
Microprocessor forms the processing part. In the temperature controller circuit, there are two parts
consisting of an LM 35 interface with ARDUINO UNO. LCD interface with ARDUINO. The hardware
circuit of the temperature controller needs the programming.


WORKING PRINCIPLE
This project consists of three sections. One senses the temperature by using a humidity and
temperature sensor namely DHT11. The second section reads the dht11 sensor module’s output
and extracts temperature value into a suitable number in Celsius scale and controls the fan
speed by using PWM. And the last part of the system shows humidity and temperature on the
LCD and Fan driver. Here we have only used this IR sensor and Temperature sensor (DHT-11)
for sensing temperature, and then programmed our arduino according to the requirements.
Working on this project is very simple. We have created PWM at the pwm pin of the arduino and
applied it at the base terminal of the transistor. Then the transistor creates a voltage according to
the PWM input. PWM is a technique by which we can control the voltage or power. To
understand it more simply, if you are applying 5 volts for driving a motor then the motor will
move with some speed, now if we reduce applied voltage by 2 means we apply 3 volts to the
motor then motor speed also decreases. This concept is used in the project to control the voltage
using PWM. (To understand more about PWM, check this circuit: 1 Watt LED Dimmer)The main
game of PWM is digital pulse with some duty cycle and this duty cycle is responsible for controlling the speed or voltage.
Suppose we have a pulse with duty cycle 50% that means it will give half of the voltage that we apply.

Formula for duty cycle given below:
Duty Cycle= Ton/T
Where T= total time or Ton+Toff
And Ton= On time of pulse (means 1 )
And Toff= Off time of pulse (means 0)

COMPONENT DESCRIPTION
Dc Motor - A DC motor is any of a class of rotary electrical motors that converts direct current
(DC) electrical energy into mechanical energy
Arduino Uno R3 - The Arduino Uno R3 is a microcontroller board based on a removable,
dual-inline-package (DIP) ATmega328 AVR microcontroller. Programs can be loaded on to it
from the easy-to-use Arduino computer program.
LCD 16 x 2 - The 16×2 LCD display is a very basic module commonly used in DIYs and circuits.
The 16×2 translates o a display 16 characters per line in 2 such lines. In this LCD each character
is displayed in a 5×7 pixel matrix.
Resistor- A passive electrical component used for either limiting or regulating the flow of
electric current in electrical circuits.
Temperature Sensor [TMP36] - a low voltage, precision centigrade temperature sensor. It
provides a voltage output that is linearly proportional to the Celsius temperature.
Relay SPDT - is a high quality Single Pole Double Throw Relay(SPDT). The Relay consists of a
coil, 1 common terminal, 1 normally closed terminal, and one normally open terminal

CODE
RESULTS

CONCLUSION
The temperature sensor was carefully chosen to gauge the room temperature. Moreover, the fan speed
will increase automatically if the temperature room is increased. In conclusion, the system which was
designed to work performed very well, for any temperature change and can be classified as automatic
control.
