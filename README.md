# Kerala IOT Challenge

> Foxlab Makerspace in association with GTech - Group of Technology Companies in Kerala is launching our prestigious program “Kerala IoT Challenge 2021”, with a vision to mould 100 IoT experts in Kerala, hosting on the µLearn platform. Kerala IoT Challenge is a program designed in 4 levels followed by a hackathon to identify and train quality industry leaders in the IoT domain, while any novice learner can start with layer 1 and others can enter laterally to the desired layer after an evaluation.
# About Me

>Hi , Iam Alan Martin,3rd year Computer Science and Engineering Student, Toc H Institute of Science and Technology,My major area of interests are IOT,Android App Development,Cyber Security and Programming 

## Experiment 1 : Hello World LED Blinking

> A basic program similar to printing "*Hello World*" in any programming language. The aim is to blink an LED using **Arduino Uno Board**.

## Components Required  
* Arduino Uno Board 
* USB Cable 
* LED (Any Color) x 1 Nos
* 220 OHM Resistor X 1 Nos
* Breadboard 
* Jumper Wires (Male to Male ) X 2 Nos

## Circuit Diagram

!(https://github.com/Alanmartin7007/Kerala-IOT-Challenge/blob/main/1.png)


## Code

int ledPin = 10; // define digital pin 10.

void setup()

{
pinMode(ledPin, OUTPUT);// define pin with LED connected as output.

}

void loop()
{

digitalWrite(ledPin, HIGH); // set the LED on.

delay(1000); // wait for a second.

digitalWrite(ledPin, LOW); // set the LED off.

delay(1000); // wait for a second

}



## Output
[[![Episode 4](https://img.youtube.com/vi/LYO3MBzF8Gk/0.jpg)](https://youtube.com/shorts/LYO3MBzF8Gk)

