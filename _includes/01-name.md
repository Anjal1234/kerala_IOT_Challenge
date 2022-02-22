# LEVEL 1
# Kerala-loT Challenge 
Fox lab Makerspace in association with GTech Group of Technology companies in Kerala is launching our prestigious program "Kerala IoT challenge 2021", with a vision to mould 100 IoT experts in Kerala, hosting on the uLearn platform. Kerala IoT Challenge is a program designed in 4 levels followed by a hackathon to identify and train quality Industry leads in the IoT domain,while any novice learner can start with layer1 and others can enter laterally to the designed layer after an evaluate

### About Me

Hi everyone! I'm ANJAL PV, 3rd year Electronic Engineering student from EKNM Government polytechnic college, Thrikarpur.I'm here to explore new dimensions of the loT world.And I also interested in App development

### Experiment 1 - Hello World LED Blinking

A basic Program similar to printing "Hello World" in any programming language. The Aim is to blink an LED using Arduino Uno Board.

Arduino Uno is an open-source microcontroller board developed by Arduino.cc. It has several advantages over the conventional microcontrollers. It comes with a pre-tested software and hardware libraries and has its own integrated development environment (IDE). Also it is less expensive & beginner friendly.
## components Required

* 680 ohm Resistor*1

* USB cable*1

* Arduino Uno*1

* Bread Board*1

* Jumper wire*2
### Circuit

![IMG_20211218_211907](https://user-images.githubusercontent.com/95326395/147376651-d3ea9f34-583e-469b-be94-e8de155b5674.jpg)
## circuit diagram
![IMG_20211225_105824](https://user-images.githubusercontent.com/95326395/147378139-54aff533-9c92-429f-8c0d-39a6723bca18.jpg)
### Code
int led1=11;
void setup()
{pinMode(11,OUTPUT);
    }
void loop()
{digitalWrite(led1,HIGH);
    delay(1000);
    digitalWrite(led1,LOW);
    delay(1000);
    }
## Video
https://user-images.githubusercontent.com/95326395/147379310-cbbf616d-55dc-478a-a860-4c87b93f3487.mp4
### Experiment 2
In the previous Experiment i have done led blinking
Now in this experiment Iam doing traffic light by using three blue leds and using three 68 ohm resistor and using jumper wires ,one bread board,one USB cable and using Arduino ide application
### components required
* Bread board*1
* Blue led*3
* Jumper wires*4
* USB cable*
* Resistor (68 ohm)*3
### circuit
![IMG_20211225_122715](https://user-images.githubusercontent.com/95326395/147379690-61065f07-bb40-477b-8c8a-1d1d79bfb18a.jpg)
### Circuit Diagram
![IMG_20211225_124620](https://user-images.githubusercontent.com/95326395/147379760-b2ef0f6b-16f0-43c3-a52a-3398e61dc0c1.jpg)
### Code
int redled = 10; 
 int yellowled=7;  
int greenled=4; 

void setup()

{

pinMode(redled, OUTPUT);
pinMode(yellowled, OUTPUT);
pinMode(greenled, OUTPUT); 

}

void loop()
{
digitalWrite(greenled, HIGH); delay(5000);

digitalWrite(greenled, LOW); 
for(int i=0;i<3;i++)
{

delay(500);
digitalWrite (yellowled, HIGH);
delay(500);
digitalWrite(yellowled, LOW);

}
 delay(500);
 digitalWrite(redled, HIGH);
 delay(5000);
digitalWrite(redled, LOW);


}

### Video
https://user-images.githubusercontent.com/95326395/147381467-8db1c727-8acf-4fe5-b0ea-8fed423e2381.mp4
# Experiment 3
## LED Chasing Effect

We often see billboards composed of colorful LEDs. They are constantly changing

to form various light effects. In this experiment, we compile a program to

simulate LED chasing effect.

The long lead of LED is the positive side; short lead is negative.
### Components Required
* Blue led*6
* Resistor*6
  (68 ohm *5,220 Ohm*1)
* Jumper Wires*7
* Arduino*1

### Circuit
![IMG_20211225_152450](https://user-images.githubusercontent.com/95326395/147382675-e5d17e3f-1994-4906-9b8b-f7a61f5c15f1.jpg)
### Circuit Diagram
![IMG_20211225_153348](https://user-images.githubusercontent.com/95326395/147382741-85bad1cb-29c7-4f73-9f97-db14fb8be0f0.jpg)
### Code
int BASE = 2;
int NUM = 6;
void setup()
{
    for (int i = BASE; i < BASE + NUM; i++)
    {
pinMode(i,OUTPUT);
    }
}
void loop()
    {
    
for (int i=BASE; i<BASE+NUM; i++)
    {
            digitalWrite(i,LOW);
        delay(200);
        }
    for (int i=BASE; i<BASE+NUM;i++)
    {
            digitalWrite(i,HIGH);
             delay(200);
        }
 }
### Video

https://user-images.githubusercontent.com/95326395/147382930-1b378595-211d-4948-8bf1-9ff0ccf72796.mp4
# Experiment 4
## Button Controlled Led
### Components Required
* Button*1
* Arduino UNO*1
* LED*1
* 220 ohm resistor*1
* 68 ohm resistor*1
* Jumper wire*6
### Circuit
![IMG_20211225_213752](https://user-images.githubusercontent.com/95326395/147389612-7d2f8ee7-d83a-4323-a7dc-a9c76fad6c8c.jpg)
### Circuit Diagram
![IMG_20211225_221736](https://user-images.githubusercontent.com/95326395/147389698-f4dd1347-a56f-49d5-be9f-c033ef71356e.jpg)
### Code
int ledpin=11;
int inpin=7;
int val;
void setup()
{
    pinMode(ledpin,OUTPUT);
    pinMode(inpin,INPUT);
    }
void loop()
{val=digitalRead(inpin);
    if(val==LOW)
    {digitalWrite(ledpin,LOW);}
    else
    {digitalWrite(ledpin,HIGH);}
    }
### Video
https://user-images.githubusercontent.com/95326395/147396223-237d81f7-fdeb-44c1-8f79-8e7762ea9c0c.mp4
# Experiment 5
### Buzzer
### Components Required
* Arduino UNO*1
* Buzzer*1
* Jumper wire*2
* Resistor (68 ohm)*1
### Circuit
![IMG_20211226_073229](https://user-images.githubusercontent.com/95326395/147397092-9c16505a-1146-489c-8351-3fc5edd73628.jpg)
### Circuit Diagram
![IMG_20211226_074013](https://user-images.githubusercontent.com/95326395/147397128-c76c50cf-e172-474f-90ea-60c06b2589fb.jpg)
### Code
int buzzer=8;

 void setup()
    {pinMode(buzzer,OUTPUT);
        }
    void loop()
    {digitalWrite(buzzer,HIGH);
        }
 
### Video
https://user-images.githubusercontent.com/95326395/147397515-d9c374cf-9f04-4b5d-86c7-bbcaa1044acb.mp4

# EXPERIMENT NO 6
## RGB LED
### COMPONENTS REQUIRED:
* ARDUINO UNO*1
* RGB LED*1
* USB CABLE*1
* JUMPER WIRE*4
* ARDUINO IDLE
### CIRCUIT
![WhatsApp Image 2022-02-22 at 10 15 45 AM](https://user-images.githubusercontent.com/95326395/155065624-bf3f22e7-4d4f-4d14-b708-9c222179c255.jpeg)
### CIRCUIT DIAGRAM
![WhatsApp Image 2022-02-22 at 10 30 59 AM](https://user-images.githubusercontent.com/95326395/155066169-2122cb74-ccac-493e-8914-c09350106e51.jpeg)

### CODE
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

## VIDEO

https://user-images.githubusercontent.com/95326395/155065951-65db58a9-4862-4397-ab1f-8303bf5e941a.mp4

# Experiment no:7
LDR interfacing with Aurdino
## Components Required
* Arduino UNO*1
* USB cable*1
* Bread board*1
* LDR*1
* LED*1
* Jumper Wires*5
### Circuit Diagram
### CODE


# Experiment no:8
 # Flame sensor interfacing with Aurdino
## Components Required
* Bread board*1
* Arduino ide
* Arduino UNO*1
* Flame sensor*1
* Buzzer*1
* Jumper Wires*5
 ## CIRCUIT DIAGRAM
 ![f7b74991-f4db-42ef-a73a-1e15f64f537d](https://user-images.githubusercontent.com/95326395/153834929-cdf97382-3b20-4b94-8249-7d796ab00a86.jpg)

## Circuit 
![WhatsApp Image 2022-02-14 at 1 45 55 PM (1)](https://user-images.githubusercontent.com/95326395/153827688-86c5f432-66fd-4da2-b00b-8386ec9806be.jpeg) 
### code

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
### video
https://user-images.githubusercontent.com/95326395/153830039-bdfc557a-ae4d-401f-b200-bfdf4dd819a0.mp4

# EXPERIMENT NO 11
## POTENTIOMETER ANALOG VALUE
## COMPONENTS REQUIRED
* ARDUINO UNO*1
* 10K POTENTIO METER*1
* BREAD BOARD *1
* JUMPER WIRE *3
* USB CABLE*1
## CIRCUIT DIAGRAM

![062c93a3-c29c-4352-b0bf-a594af793d22](https://user-images.githubusercontent.com/95326395/154444477-c253c541-4a12-4084-bf41-279568b45254.jpg)


## CODE 
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

### CIRCUIT
![86c82790-ccf7-4a4c-94e0-a4aef7c639cc](https://user-images.githubusercontent.com/95326395/154444195-182a43ba-8a08-413a-b27e-4e323508cb4f.jpg)

### VIDEO
https://user-images.githubusercontent.com/95326395/154443314-102e6cc6-760d-4486-8346-5815c332ce95.mp4

# EXPERIMENT NO 12
## 7 SEGMENT DISPLAY
## COMPONENTS REQUIRED
* ARDUINO UNO BOARD*1
* 1-DIGIT LED SEGMENT DISPLAY*1
* 220 OHM RESISTOT
* BREAD BOARD*1
* JUMPER*SEVERAL
* USB CABLE*1
## CIRCUIT DIAGRAM
![138b5870-8ee8-4c28-b94c-58640891708e](https://user-images.githubusercontent.com/95326395/153834832-3542c4c9-1293-407e-a85a-bef6100440d6.jpg)

## CODE
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
### CIRCUIT
![WhatsApp Image 2022-02-14 at 1 45 54 PM](https://user-images.githubusercontent.com/95326395/153832737-1c226d65-7db9-47cf-8b26-506803c25310.jpeg)
### VIDEO


https://user-images.githubusercontent.com/95326395/153833527-0c8a05cb-a3b1-44c8-9e69-5724f5b409e7.mp4


