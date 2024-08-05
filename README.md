# Tinkercad_mini_Projects
I will be sharing all my tinkercad_mini_projects in this repository.

### Distance_with_Ultrasonic_sensor

#### Setup Phase:

The program initializes by starting a serial communication with a specific baud rate, which allows the Arduino to send data to the computer.
Two pins are designated for the ultrasonic sensor: one for sending the signal (trigger) and one for receiving the echo (echo).

#### Measurement Loop:

1. The program continuously measures distance in a loop.
2. It first ensures the trigger pin is low, then briefly sets it high and low again to create an ultrasonic pulse.
3. The sensor sends out an ultrasonic burst and waits for it to bounce back.
T4. he time taken for the pulse to return is measured.
Using this time, the program calculates the distance to an object based on the speed of sound.
5. The distance is then sent to the serial monitor to be displayed on the computer screen.
6. There is a short delay before the next measurement cycle begins, ensuring readings are taken at regular intervals.