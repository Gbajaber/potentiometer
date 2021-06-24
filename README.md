# potentiometer
controlling the servo motor by potentiometer


This project is considered as required by smart methods company in cooperative training for the year 2021 controlling servo motor

Tinkercad is the website that used to create servos motor circuit

The objective to control the motors by potentiometer

componets: Arduino Uno R3 = 1 Positional Micro Servo = 5 potentiometer =5

the code

#include <Servo.h> 
Servo my_servo;
Servo my_servo1;
Servo my_servo2;
Servo my_servo3;
Servo my_servo4;
Servo my_servo5;

int pot_pin = 0;
int pot_pin1 = 1;
int pot_pin2 = 2;
int pot_pin3 = 3;
int pot_pin4 = 4;


int val;
int val5;
int val2;
int val3;
int val4;

void setup()
{
  my_servo.attach(3);
  my_servo1.attach(5);
  my_servo2.attach(6);
  my_servo3.attach(9);
  my_servo4.attach(10);
}
void loop()
{
  val = analogRead(pot_pin);
  val = map (val , 0 , 1023 , 0 , 180) ;
  my_servo.write(val);
  delay(15);
  
  val5 = analogRead(pot_pin1);
  val5 = map (val5 , 0 , 1023 , 0 , 180) ;
  my_servo1.write(val5);
  delay(15);
  
  val2 = analogRead(pot_pin2);
  val2 = map (val2 , 0 , 1023 , 0 , 180) ;
  my_servo2.write(val2);
  delay(15);
  
  val3 = analogRead(pot_pin3);
  val3 = map (val3 , 0 , 1023 , 0 , 180) ;
  my_servo3.write(val3);
  delay(15);
  
   val4 = analogRead(pot_pin4);
  val3 = map (val4 , 0 , 1023 , 0 , 180) ;
  my_servo4.write(val4);
  delay(15);
  }
  
tinkercad link

https://www.tinkercad.com/things/1PNOxG0mwq2-potentiometer/editel
