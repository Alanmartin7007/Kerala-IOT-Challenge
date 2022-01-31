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

[![video](https://img.youtube.com/vi/S9a0FcGu3Fw/0.jpg)](https://youtube.com/shorts/S9a0FcGu3Fw)


## Experiment 6 -RGB LED

### Components
* Arduino Uno
* Breadboard
* RGB LED
* Jumper wire
* Restsor 220 ohm 

### Circuit Diagram

![Image](https://github.com/Alanmartin7007/Kerala-IOT-Challenge/blob/main/6.png)

### Code

int redpin = 11; //select the pin for the red LED

int bluepin =10; // select the pin for the blue LED

int greenpin =9;// select the pin for the green LED

int val;

void setup() {

pinMode(redpin, OUTPUT);

pinMode(bluepin, OUTPUT);

pinMode(greenpin, OUTPUT);

Serial.begin(9600);

}

void loop() 

{

for(val=255; val>0; val--)

{

analogWrite(11, val);

analogWrite(10, 255-val);

analogWrite(9, 128-val);

delay(1); 

}

for(val=0; val<255; val++)

{

analogWrite(11, val);

analogWrite(10, 255-val);

analogWrite(9, 128-val);

delay(1); 

}

Serial.println(val, DEC);

}


### Output

[![video](https://img.youtube.com/vi/_qaTREAmWR8/0.jpg)](https://www.youtube.com/shorts/_qaTREAmWR8)


### Experiment 7 : LDR Light Sensor

### Components Required 

*Arduino Uno Board
*Photo Resistor*1
*Red M5 LED*1
*10KΩ Resistor*1
*220Ω Resistor*1
*Breadboard*1
*Breadboard Jumper Wire*5
*USB cable*1

### Circuit Diagram

![image](https://github.com/Alanmartin7007/Kerala-IOT-Challenge/blob/main/7.png)

### Code

int potpin=0;// initialize analog pin 0, connected with photovaristor

int ledpin=11;// initialize digital pin 11, 

int val=0;// initialize variable val

void setup()

{

pinMode(ledpin,OUTPUT);// set digital pin 11 as “output”

Serial.begin(9600);// set baud rate at “9600”

}

void loop()

{

val=analogRead(potpin);// read the value of the sensor and assign it to val

Serial.println(val);// display the value of val

analogWrite(ledpin,val/4);// set up brightness（maximum value 255）

delay(10);// wait for 0.01 

}


### Output

[![video](https://img.youtube.com/vi/5ACuo1C0Xhw/0.jpg)](https://www.youtube.com/shorts/5ACuo1C0Xhw)


## Experiment  8- FLAME SENSOR 

### Components

* Arduino Uno
* Breadboard
* RED LED
* BUZZER
* Jumper wire
* Restsor 220 ohm 10 k
* Flame Sensor

### Circuit Diagram 
![image](https://github.com/Alanmartin7007/Kerala-IOT-Challenge/blob/main/8.png)

### Code


int flame=0;// select analog pin 0 for the sensor

int Beep=9;// select digital pin 9 for the buzzer

int val=0;// initialize variable

void setup() 

{

pinMode(Beep,OUTPUT);// set LED pin as “output”

pinMode(flame,INPUT);// set buzzer pin as “input”

Serial.begin(9600);// set baud rate at “9600”

} 

void loop() 

{ 

val=analogRead(flame);// read the analog value of the sensor 

Serial.println(val);// output and display the analog value

if(val>=600)// when the analog value is larger than 600, the buzzer will buzz

{  

digitalWrite(Beep,HIGH); 

}else 

{  

digitalWrite(Beep,LOW); 

}

delay(500); 


}


### Output

[![Video](https://img.youtube.com/vi/WSL2B_O7FpA/0.jpg)](https://www.youtube.com/shorts/WSL2B_O7FpA)

## Experiment  9- LM35 Temperature Sensor

### Component's 

*Arduino Uno  Board*1
*LM35*1
*Breadboard*1
*Breadboard Jumper Wire*5
*USB cable

### Circuit Digram

![image](https://github.com/Alanmartin7007/Kerala-IOT-Challenge/blob/main/9.png)

### Code


int potPin = 0; // initialize analog pin 0 for LM35 temperature sensor

void setup()

{

Serial.begin(9600);// set baud rate at”9600”

}

void loop()


{

int val;// define variable

int dat;// define variable



val=analogRead(0);// read the analog value of the sensor and assign it to val

dat=(125*val)>>8;// temperature calculation formula


Serial.print("Tep");// output and display characters beginning with Tep

Serial.print(dat);// output and display value of dat

Serial.println("C");// display “C” characters

delay(500);// wait for 0.5 second

}


### Output

[![video]((https://img.youtube.com/vi/0Aj8wgyUiVM/0.jpg)](https://www.youtube.com/shorts/0Aj8wgyUiVM)


## Experiment  10- IR Remote Control Using TSOP

### Components

* Arduino Uno
* Breadboard
* Jumper wire
* IR Recever (TSOP)
* 5 LED
* 220 ohm Resistor
* IR REMOTE (Any remote)


### Circuit Diagram

![image](https://github.com/Alanmartin7007/Kerala-IOT-Challenge/blob/main/10.png)

### Code


#include <IRremote.h>

int RECV_PIN = 11;

int LED1 = 2;

int LED2 = 3;

int LED3 = 4;

int LED4 = 5;

int LED5 = 6;

int LED6 = 7;

long on1  = 0x00FF6897;

long off1 = 0x00FF9867;

long on2 = 0x00FFB04F;

long off2 = 0x00FF30CF;

long on3 = 0x00FF18E7;

long off3 = 0x00FF7A85;

long on4 = 0x00FF10EF;

long off4 = 0x00FF38C7;

long on5 = 0x00FF5AA5;

long off5 = 0x00FF42BD;

long on6 = 0x00FF4AB5;

long off6 = 0x00FF52AD;

IRrecv irrecv(RECV_PIN);

decode_results results;

// Dumps out the decode_results structure.

// Call this after IRrecv::decode()

// void * to work around compiler issue

//void dump(void *v) {

//  decode_results *results = (decode_results *)v

void dump(decode_results *results) {

int count = results->rawlen;

if (results->decode_type == UNKNOWN) 

{

Serial.println("Could not decode message");

} 

else 

{

if (results->decode_type == NEC) 

{

Serial.print("Decoded NEC: ");

} 

else if (results->decode_type == SONY) 

{

Serial.print("Decoded SONY: ");

} 

else if (results->decode_type == RC5) 

{

Serial.print("Decoded RC5: ");

} 

else if (results->decode_type == RC6) 

{

Serial.print("Decoded RC6: ");

}

Serial.print(results->value, HEX);

Serial.print(" (");

Serial.print(results->bits, DEC);

Serial.println(" bits)");

}

Serial.print("Raw (");

Serial.print(count, DEC);

Serial.print("): ");

for (int i = 0; i < count; i++) 

{

if ((i % 2) == 1) {

Serial.print(results->rawbuf[i]*USECPERTICK, DEC);

} 

else  

{

Serial.print(-(int)results->rawbuf[i]*USECPERTICK, DEC);

}

Serial.print(" ");

}

Serial.println("");

}

void setup()

{

pinMode(RECV_PIN, INPUT);   

pinMode(LED1, OUTPUT);

pinMode(LED2, OUTPUT);

pinMode(LED3, OUTPUT);

pinMode(LED4, OUTPUT);

pinMode(LED5, OUTPUT);

pinMode(LED6, OUTPUT);  

pinMode(13, OUTPUT);

Serial.begin(9600);

irrecv.enableIRIn(); // Start the receiver

}

int on = 0;

unsigned long last = millis();

void loop() 

{

if (irrecv.decode(&results)) 

{

// If it's been at least 1/4 second since the last

// IR received, toggle the relay

if (millis() - last > 250) 

{

on = !on;

//       digitalWrite(8, on ? HIGH : LOW);


digitalWrite(13, on ? HIGH : LOW);

dump(&results);
      }

if (results.value == on1 )

digitalWrite(LED1, HIGH);

if (results.value == off1 )


digitalWrite(LED1, LOW); 

if (results.value == on2 )

digitalWrite(LED2, HIGH);

if (results.value == off2 )

digitalWrite(LED2, LOW); 

if (results.value == on3 )

digitalWrite(LED3, HIGH);

if (results.value == off3 )


digitalWrite(LED3, LOW);

if (results.value == on4 )

digitalWrite(LED4, HIGH);

if (results.value == off4 )

digitalWrite(LED4, LOW); 

if (results.value == on5 )

digitalWrite(LED5, HIGH);

if (results.value == off5 )

digitalWrite(LED5, LOW); 

if (results.value == on6 )

digitalWrite(LED6, HIGH);

if (results.value == off6 )

digitalWrite(LED6, LOW);        

last = millis();      


irrecv.resume(); // Receive the next value

}

}



### Output

[![video](https://img.youtube.com/vi/ZAFLklsKFw8/0.jpg)](https://www.youtube.com/watch?v=ZAFLklsKFw8)



## Exp 11 :Potentiometer analog Value Reading

### Components Required 

*Arduino Uno Board*1]

*10K Potentiometer *1

*Breadboard*1

*Breadboard Jumper Wire*3

*USB cable*1

### Circuit Diagram

![Image](https://github.com/Alanmartin7007/Kerala-IOT-Challenge/blob/main/11.png)

### Code
int potpin=0;// initialize analog pin 0

int ledpin=13;// initialize digital pin 13

int val=0;// define val, assign initial value 0

void setup()

{

pinMode(ledpin,OUTPUT);// set digital pin as “output”

Serial.begin(9600);// set baud rate at 9600

}

void loop()

{

digitalWrite(ledpin,HIGH);// turn on the LED on pin 13

delay(50);// wait for 0.05 second


digitalWrite(ledpin,LOW);// turn off the LED on pin 13

delay(50);// wait for 0.05 second

val=analogRead(potpin);// read the analog value of analog pin 0, and assign it to val 

Serial.println(val);// display val’s value

}



### OUTPUT

![IMAGE](https://github.com/Alanmartin7007/Kerala-IOT-Challenge/blob/main/o11.jpeg)
![IMAGE](https://github.com/Alanmartin7007/Kerala-IOT-Challenge/blob/main/o11a.jpeg)

## Experiment  12- Seven Segment Display

### Components

* Arduino Uno
* Breadboard
* Seven Segment Display
* Jumper wire
* Restsor 220 ohm

### Circuit Diagram

![image](https://github.com/Alanmartin7007/Kerala-IOT-Challenge/blob/main/12.png)

### Code

int a=7;// set digital pin 7 for segment a

int b=6;// set digital pin 6 for segment b

int c=5;// set digital pin 5 for segment c

int d=10;// set digital pin 10 for segment d

int e=11;// set digital pin 11 for segment e

int f=8;// set digital pin 8 for segment f

int g=9;// set digital pin 9 for segment g

int dp=4;// set digital pin 4 for segment dp

void digital_0(void) // display number 5

{

unsigned char j;

digitalWrite(a,HIGH);

digitalWrite(b,HIGH);

digitalWrite(c,HIGH);

digitalWrite(d,HIGH);

digitalWrite(e,HIGH);

digitalWrite(f,HIGH);

digitalWrite(g,LOW);

digitalWrite(dp,LOW);

}

void digital_1(void) // display number 1

{

unsigned char j;

digitalWrite(c,HIGH);// set level as “high” for pin 5, turn on segment c

digitalWrite(b,HIGH);// turn on segment b

for(j=7;j<=11;j++)// turn off other segments

digitalWrite(j,LOW);

digitalWrite(dp,LOW);// turn off segment dp

}


void digital_2(void) // display number 2

{

unsigned char j;

digitalWrite(b,HIGH);

digitalWrite(a,HIGH);

for(j=9;j<=11;j++)

digitalWrite(j,HIGH);

digitalWrite(dp,LOW);


digitalWrite(c,LOW);

digitalWrite(f,LOW);

}

void digital_3(void) // display number 3

{digitalWrite(g,HIGH);

digitalWrite(a,HIGH);

digitalWrite(b,HIGH);

digitalWrite(c,HIGH);

digitalWrite(d,HIGH);

digitalWrite(dp,LOW);


digitalWrite(f,LOW);

digitalWrite(e,LOW);

}

void digital_4(void) // display number 4

{digitalWrite(c,HIGH);

digitalWrite(b,HIGH);

digitalWrite(f,HIGH);

digitalWrite(g,HIGH);

digitalWrite(dp,LOW);

digitalWrite(a,LOW);

digitalWrite(e,LOW);

digitalWrite(d,LOW);

}

void digital_5(void) // display number 5


{

unsigned char j;

digitalWrite(a,HIGH);

digitalWrite(b, LOW);

digitalWrite(c,HIGH);

digitalWrite(d,HIGH);

digitalWrite(e, LOW);

digitalWrite(f,HIGH);

digitalWrite(g,HIGH);

digitalWrite(dp,LOW);

}

void digital_6(void) // display number 6

{

unsigned char j;

for(j=7;j<=11;j++)

digitalWrite(j,HIGH);

digitalWrite(c,HIGH);

digitalWrite(dp,LOW);

digitalWrite(b,LOW);

}

void digital_7(void) // display number 7

{

unsigned char j;

for(j=5;j<=7;j++)

digitalWrite(j,HIGH);

digitalWrite(dp,LOW);

for(j=8;j<=11;j++)

digitalWrite(j,LOW);

}

void digital_8(void) // display number 8

{

unsigned char j;

for(j=5;j<=11;j++)

digitalWrite(j,HIGH);

digitalWrite(dp,LOW);

}

void digital_9(void) // display number 5

{

unsigned char j;

digitalWrite(a,HIGH);


digitalWrite(b,HIGH);

digitalWrite(c,HIGH);


digitalWrite(d,HIGH);

digitalWrite(e, LOW);


digitalWrite(f,HIGH);

digitalWrite(g,HIGH);


digitalWrite(dp,LOW);



}

void setup()

{

int i;// set variable

for(i=4;i<=11;i++)

pinMode(i,OUTPUT);// set pin 4-11as “output”

}

void loop()

{

while(1)

{

digital_0();// display number 0

delay(1000);// wait for 1s

digital_1();// display number 1

delay(1000);// wait for 1s

digital_2();// display number 2

delay(1000); // wait for 1s

digital_3();// display number 3

delay(1000); // wait for 1s

digital_4();// display number 4

delay(1000); // wait for 1s

digital_5();// display number 5

delay(1000); // wait for 1s

digital_6();// display number 6

delay(1000); // wait for 1s

digital_7();// display number 7
delay(1000); // wait for 1s


digital_8();// display number 8

delay(1000); // wait for 1s

digital_9();// display number 9

delay(1000); // wait for 1s

}}


### Output

[![video](https://img.youtube.com/vi/Dt3fECPXsAs/0.jpg)](https://www.youtube.com/watch?v=Dt3fECPXsAs)

## Assignment 1

### Create an automatic night lamp model using LDR and LED

### Components
* Arduino Uno
* Breadboard
* RED,GREEN LED
* Jumper wire
* Restsor 220 ohm 10 k
* LDR Senso

### Code

#define LDR A0// LDR CONNECT A0

#define LED 11 // LED CONNECT 11

int readData=0;

void setup(){ 

pinMode(LED,OUTPUT);

pinMode(LDR,INPUT);

Serial.begin(9600);


} 
void loop(){

readData=analogRead(LDR);

Serial.println(readData);

if(readData>200)

digitalWrite(LED,HIGH);

else


digitalWrite(LED,LOW);

}


### Output

[![video](https://img.youtube.com/vi/Gc0iOuvF9e0/0.jpg)](https://www.youtube.com/shorts/Gc0iOuvF9e0)

## Assignment 2

### Create a Digital Dice using 6 LEDs and 1 Push Button

### Components Required 

### Components
* Arduino Uno
* Breadboard
* pushbuttion
* Jumper wire
* Restsor 220 ohm
* push buttion


### Code

int triggerButton = 2;


int bottomLeftLED = 3;

int middleLeftLED = 4;

int upperLeftLED = 5;

int middleLED = 6;

int bottomRightLED = 7;

int upperRight = 8;

long randomDiceNumber;

void setup(){

// set all of the LED pins to OUTPUT

pinMode(bottomLeftLED, OUTPUT);

pinMode(middleLeftLED, OUTPUT);

pinMode(upperLeftLED, OUTPUT);

pinMode(middleLED, OUTPUT);

pinMode(bottomRightLED, OUTPUT);

pinMode(upperRight, OUTPUT);



// set the button to INPUT

pinMode(triggerButton, INPUT);



// create a seed for our random numbers

randomSeed(analogRead(0));

}
void loop(){

//Read our triggerButton if high then run dice

if (digitalRead(triggerButton) == HIGH){



// give the impression the dice is "thinking" by cycling numbers 5 times quickly

// (yes, this routing could be written in two lines, but I left it this way to make it simple to undestand)

for (int i=0; i <= 5; i++){

MakeOne();

delay(60);

clearDice();

MakeTwo();

delay(60);

clearDice();

MakeThree();

delay(60);

clearDice();


MakeFour();

delay(60);

clearDice();

MakeFive();

delay(60);

clearDice();

MakeSix();

delay(60);

clearDice();

delay(60);


}

// pause 300ms blank before selecting and showing the number

delay(300);



randomDiceNumber = random(1, 7);

delay(100);

Serial.println(randomDiceNumber);



if (randomDiceNumber == 6){

MakeSix();

}

if (randomDiceNumber == 5){

MakeFive();

}

if (randomDiceNumber == 4){

MakeFour();

}

if (randomDiceNumber == 3){

MakeThree();

}

if (randomDiceNumber == 2){

MakeTwo();

}

if (randomDiceNumber == 1){

MakeOne();

}

delay(5000);

clearDice();
    }



}
 

// Thes functions create our dice



// make a six

void MakeSix()

{

digitalWrite(bottomLeftLED, HIGH);

digitalWrite(middleLeftLED, HIGH);

digitalWrite(upperLeftLED, HIGH);

digitalWrite(bottomRightLED, HIGH);

digitalWrite(upperRight, HIGH);

}



// make a five
void MakeFive()

{

digitalWrite(upperLeftLED, HIGH);

digitalWrite(bottomLeftLED, HIGH);

digitalWrite(middleLED, HIGH);

digitalWrite(upperRight, HIGH);

digitalWrite(bottomRightLED, HIGH);

}



// make a four

void MakeFour()

{

digitalWrite(upperLeftLED, HIGH);

digitalWrite(bottomLeftLED, HIGH);

digitalWrite(upperRight, HIGH);

digitalWrite(bottomRightLED, HIGH);

}



//make a three

void MakeThree()

{

digitalWrite(upperLeftLED, HIGH);

digitalWrite(middleLED, HIGH);

digitalWrite(bottomRightLED, HIGH);

}



// make a two

void MakeTwo()

{

digitalWrite(bottomRightLED, HIGH);

digitalWrite(upperLeftLED, HIGH);

}



// make a one

void MakeOne(){

digitalWrite(middleLED, HIGH);

}



// This routine clears the dice back to zero

void clearDice(){

digitalWrite(bottomLeftLED, LOW);

digitalWrite(middleLeftLED, LOW);

digitalWrite(upperLeftLED, LOW);



digitalWrite(middleLED,LOW);

digitalWrite(bottomRightLED, LOW);

digitalWrite(upperRight, LOW);

}





### Output


[![video](https://img.youtube.com/vi/bepJdfCxvlY/0.jpg)](https://www.youtube.com/shorts/bepJdfCxvlY)
