
# Kerala-loT Challenge 
Fox lab Makerspace in association with GTech Group of Technology companies in Kerala is launching our prestigious program "Kerala IoT challenge 2021", with a vision to mould 100 IoT experts in Kerala, hosting on the uLearn platform. Kerala IoT Challenge is a program designed in 4 levels followed by a hackathon to identify and train quality Industry leads in the IoT domain,while any novice learner can start with layer1 and others can enter laterally to the designed layer after an evaluate

### About Me

Hi everyone! I'm ANJAL PV, 3rd year Electronic Engineering student from EKNM Government polytechnic college, Thrikarpur.I'm here to explore new dimensions of the loT world.And I also interested in App development

### Experiment 1 - Hello World LED Blinking

A basic Program similar to printing "Hello World" in any programming language. The Aim is to blink an LED using Arduino Uno Board.

Arduino Uno is an open-source microcontroller board developed by Arduino.cc. It has several advantages over the conventional microcontrollers. It comes with a pre-tested software and hardware libraries and has its own integrated development environment (IDE). Also it is less expensive & beginner friendly.
## components Required

*680 ohm Resistor*1

*USB cable*1

*Arduino Uno*1

*Bread Board*1

*Jumper wire*2

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
