# Exam

## About the project:
This project is about using DAC to create a square signal wave with different slew rate and use ADC to detect and sample
it, then plot the wave by Matplotlib with the ADC datas.
## Built with:
C++, Python
## Description
This project is embedding in B_L4S5I_IOT01A, the inputs are three buttons that can select the slew rate of the output 
wave, which are up down and confirm respectively.
When the "up" button is pressed, it execute to a function that can let a variable plus one, and the variable minus 
one when the "down" button is pressed. 
The current frequency is shown on the uLCD, when the "confirm" button is pressed, it execute the loop that can generate
square wave with the current slew rate.
In the loop, it save a data point in a matrix when a input point is generated. 
In this code, the matrix save the data points of two period of the triangle wave, and we have it print it out. 
Thus as soon as the "confirm" button is pressed, we can see the signal through picoscope by the command "picoscope &". 
Then run "sudo python3 FFT.py" first to start to plot the Matplotlib, then pressed the "confirm" button to complete.
