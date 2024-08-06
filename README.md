# Tinkercad_mini_Projects
I will be sharing all my tinkercad_mini_projects in this repository.

### Distance_with_Ultrasonic_sensor

#### Setup Phase:

1. The program initializes by starting a serial communication with a specific baud rate, which allows the Arduino to send data to the computer.
2. Two pins are designated for the ultrasonic sensor: one for sending the signal (trigger) and one for receiving the echo (echo).

#### Measurement Loop:

1. The program continuously measures distance in a loop.
2. It first ensures the trigger pin is low, then briefly sets it high and low again to create an ultrasonic pulse.
3. The sensor sends out an ultrasonic burst and waits for it to bounce back.
T4. he time taken for the pulse to return is measured.
Using this time, the program calculates the distance to an object based on the speed of sound.
5. The distance is then sent to the serial monitor to be displayed on the computer screen.
6. There is a short delay before the next measurement cycle begins, ensuring readings are taken at regular intervals.

### Temperature_sensor_reading

1. The serial communication is started at a baud rate of 9600 to allow data to be sent to the computer for monitoring.
2. The pin connected to the LM35 sensor (A0) is set up as an input.

#### Reading and Converting the Sensor Data:

1. In a loop, the code continuously reads the analog value from the LM35 sensor.
2. This analog value is then converted to a temperature in Celsius. The conversion factor is derived from the sensor's characteristics, where the output voltage is linearly proportional to the temperature in Celsius.
3. The temperature in Celsius is then converted to Fahrenheit.

#### Displaying the Data:

1. The temperature values in both Celsius and Fahrenheit are printed to the serial monitor.
2. A delay of one second is included to space out the readings.
