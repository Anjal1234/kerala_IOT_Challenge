
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
