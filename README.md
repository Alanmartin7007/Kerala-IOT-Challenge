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

![Expriment 1](https://github.com/Alanmartin7007/Kerala-IOT-Challenge/blob/main/1.png)


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
[[![video1](https://img.youtube.com/vi/LYO3MBzF8Gk/0.jpg)](https://youtube.com/shorts/LYO3MBzF8Gk)



## Experiment 2 - Traffic Light
### Components
* Arduino Uno
* Breadboard
* LED RED BLUE GREEN
* Jumper wire
* Restsor 220 ohm

### Circuit
![Expriment 2](https://github.com/Alanmartin7007/Kerala-IOT-Challenge/blob/main/2.png)


### Code

int redled =10; // initialize digital pin 8.

int yellowled =7; // initialize digital pin 7.

int greenled =4; // initialize digital pin 4.

void setup()

{

pinMode(redled, OUTPUT);// set the pin with red LED as “output”

pinMode(yellowled, OUTPUT); // set the pin with yellow LED as “output”

pinMode(greenled, OUTPUT); // set the pin with green LED as “output”

}

void loop()

{

digitalWrite(greenled, HIGH);//// turn on green LED

delay(5000);// wait 5 seconds



digitalWrite(greenled, LOW); // turn off green LED

for(int i=0;i<3;i++)// blinks for 3 times

{

delay(500);// wait 0.5 second

digitalWrite(yellowled, HIGH);// turn on yellow LED

delay(500);// wait 0.5 second

digitalWrite(yellowled, LOW);// turn off yellow LED

} 

delay(500);// wait 0.5 second

digitalWrite(redled, HIGH);// turn on red LED

delay(5000);// wait 5 seconds

digitalWrite(redled, LOW);// turn off red LED

}


###output

[[![video1](https://img.youtube.com/vi/xx9oFRN1428/0.jpg)](https://youtube.com/shorts/xx9oFRN1428)


## Experiment 3 - LED Chasing Effect

### Components

* Arduino Uno
* Breadboard
* LED 6
* Jumper wire
* Restsor 220 oh

### Circuit Diagram

![Expriment 3](https://github.com/Alanmartin7007/Kerala-IOT-Challenge/blob/main/3.png)

### Code

int redled =10; // initialize digital pin 8.

int yellowled =7; // initialize digital pin 7.

int greenled =4; // initialize digital pin 4.

void setup()

{

pinMode(redled, OUTPUT);// set the pin with red LED as “output”

pinMode(yellowled, OUTPUT); // set the pin with yellow LED as “output”

pinMode(greenled, OUTPUT); // set the pin with green LED as “output”

}

void loop()

{

digitalWrite(greenled, HIGH);//// turn on green LED

delay(5000);// wait 5 seconds



digitalWrite(greenled, LOW); // turn off green LED

for(int i=0;i<3;i++)// blinks for 3 times

{

delay(500);// wait 0.5 second

digitalWrite(yellowled, HIGH);// turn on yellow LED

delay(500);// wait 0.5 second

digitalWrite(yellowled, LOW);// turn off yellow LED

} 

delay(500);// wait 0.5 second

digitalWrite(redled, HIGH);// turn on red LED

delay(5000);// wait 5 seconds

digitalWrite(redled, LOW);// turn off red LED

}


### output

[[![video1](https://img.youtube.com/vi/feebf7U-Txk/0.jpg)](https://youtube.com/shorts/feebf7U-Txk?feature=play)


## Experiment 4 -Button Controlled LED


### Components

*Arduino Uno
*Button switch*1
*Red M5 LED*1
*220ΩResistor*1
*10KΩ Resistor*1
*Breadboard*1
*Breadboard Jumper Wire*6
*USB cable*1

### Circuit Diagram


![image](https://github.com/Alanmartin7007/Kerala-IOT-Challenge/blob/main/4.png)

### Code


int ledpin=11;// initialize pin 11

int inpin=7;// initialize pin 7

int val;// define val

void setup()

{

pinMode(ledpin,OUTPUT);// set LED pin as “output”

pinMode(inpin,INPUT);// set button pin as “input”

}

void loop()

{

val=digitalRead(inpin);// read the level value of pin 7 and assign if to val

if(val==LOW)// check if the button is pressed, if yes, turn on the LED

{ digitalWrite(ledpin,LOW);}

else

{ digitalWrite(ledpin,HIGH);}

}



### Output

[![video](https://img.youtube.com/vi/THfPDleDF7Y/0.jpg)](https://youtube.com/shorts/THfPDleDF7Y)



## Experiment 5 -BUZZER

### Components

*Arduino Uno
*Buzzer*1
*Breadboard*1
*Breadboard Jumper Wire*2
*USB cable*1

### Circuit Diagram

![image](https://github.com/Alanmartin7007/Kerala-IOT-Challenge/blob/main/5.png)

### Code

int buzzer=8;// initialize digital IO pin that controls the buzzer

void setup() 

{ 

pinMode(buzzer,OUTPUT);// set pin mode as “output”

} 

void loop() 

{

digitalWrite(buzzer, HIGH); // produce sound

}


### Output

[![video](https://img.youtube.com/vi/G_p7adSctlQ/0.jpg)](https://youtube.com/shorts/S9a0FcGu3Fw)

