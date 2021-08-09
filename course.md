<!--
author:   Abeer Abusobaih

email:    aabusobaih@gmail.com

version:  0.0.1

language: en

narrator:  US English Female

comment:  Try to write a short comment about
          your course, multiline is also okay.

link:     https://cdn.jsdelivr.net/chartist.js/latest/chartist.min.css

script:   https://cdn.jsdelivr.net/chartist.js/latest/chartist.min.js

import:   https://raw.githubusercontent.com/liaTemplates/AVR8js/main/README.md

-->

# Arduino Course

<br/>

<br/>

<br/>

**Title** :  Arduino for Beginners

<br/>

**Grade Level** :  School's students up to 10 years old

<br/>

**Objective of the Course** :

1. To engage and motivate schools student's interest in learning and creating their own electronics with Arduino.
2. To give students more confidence to ask questions and the tools to find the answers and to solve a real-life  problems using hand-on training.

<br/>

**After completing this course students will be able to:**

1. To have the knowledge of the most common hardware components and their usage in electronic circuits.
2. To  write Arduino programs.
3. To create your own projects.

<br/>


**Previous Knowledge**

This course is designed for students who have no or a very little prior experience in electronics and programming.

<br/>

<br/>

![image example](pic/main.jfif)

## Introduction
<br/>

**Course Description:**

1. Are you interested to build a project using Arduino?
2. Do you want to know and learn everything related to Arduino?
3. Do you want to understand the code load on an Arduino?
4. Do you wish you had a clear path to learn an Arduino?
<br/>

If you answered yes to one or more of the questions above, then you are the person we are trying to help with our course.
<br/>

We know the learning path is not easy, you get stuck sometime, then unstuck and so on ... because of that we designed this course to make you understand in very simple and easy way.

Our course have step-by-step instruction, but still it requires from you to exercise your brain, and we challenge you to make your ideas and think how to apply them according to what you have learnt.  

We designed this course to take you from no knowledge about programming, to being able to understand how to write your own programs for the Arduino projects. To know an exact component to use, and how this component work and connect to microcontroller.

We want to design a path that you can follow, to develop your skills.

## What is an Arduino
<br/>

Have you heard about Arduino ? or have you seen some projects that use an Arduino ?
<br/>

So, **What is an Arduino ?**

<br/>

  ![image example](pic/jj.jpg)

  <br/>


  let's start by understanding the core principles of an Arduino using an example:
  let's say we have a smart house which is equipped with automated lights, this house checks the light intensity of the environment and turns on at night and turns off during the day.


![image example](pic/R.jfif)  <br/> <br/> <br/> <br/> <br/>  ~~So what sort of equipment would be required to build such a system ?!~~

You need a light,  light sensor to give us information of the ambient light, and something in between that gets the input from the light sensor and outputs the signal to the light, this something is the brain of the system, and it called a microcontroller unit.

microcontroller like a small computer that can handle small amounts of information fast, and **Arduino** is a company that produces microcontroller boards, they have different versions of microcontroller boards that provide different scenarios but, the most commonly used is the Arduino Uno, the main difference is the size, capacity, and number of pins.

*Arduino* is an open source electronics platform based on easy to use hardware and software, and can be programmed with an Arduin IDE. [1](https://www.arduino.cc/en/guide/introduction)

**Arduino** consists of both a physical programmable circuit board and a piece of software, or IDE.

<br/>

**Why Arduino?**
<br/>

+ The Arduino software is published as open source tools, available for extension by experienced programmers.
+ Arduino designed a microcontroller that is so easy to use from somebody without any prior electronics or programming knowledge.
+ So popular and easy to use.
<br/>

**How does Arduino Work?**
<br/>

Arduino Hardware
![image example](pic/hello.jpg)

Arduino IDE
 ![image example](pic/IDE.png)

 Arduino Code
  ![image example](pic/code.png)




## Getting Started

This chapter provides an overview of what you need to get started with Arduino.

## Arduino Hardware

<br/> <br/> <br/> <br/> <br/>
![image example](pic/hw.jpg)
#### The Arduino UNO
<br/>

The UNO is one of the more popular boards in the Arduino family and a great choice for beginners.
<br/>



 *The major components of the Arduino UNO board are the following*
 <br/>
 <br/>

![image example](pic/micro.png)
<br/>

USB Connecter: used to load a program from the Arduino IDE onto the Arduino board, and to give power to the board.
<!-- class = "animated rollIn" style = "animation-delay: 3s; color: green" -->
Power Port: the Arduino board can be powered through a AC to DC adapter.
<!-- class = "animated rollIn" style = "animation-delay: 3s; color: darkred " -->
Microcontroller: It's as the barin of the Arduino, it is like a small computer it has a 28 pins. The Microcontroller used on the UNO board is Atmega328P, and it has the following components in it:
<br/>
+ Flash memory of 32KB, the program loaded from the Arduino IDE is stored here.
<br/>
+ RAM of 2KB. <br/>
+ CPU. It controls everything that goes on within the device.<br/>
+ Electrically Erasable Programmable Read Only Memory (EEPROM), it keeps the data even after device restart and reset.

<!-- class = "animated rollIn" style = "animation-delay: 3s; color: purple" -->
Analog Input pins: There are 6 pins, labeled as "ANALOG A0-A5", used to read the signal from an analog sensor such as the temperature sensor. It converts the analog signal to digital value to make system understand it.
Those pins just measure voltage, only a small amount of current flows through them.

 <!-- class = "animated rollIn" style = "animation-delay: 3s; color: red" -->
Digital pins: They are labeled as "DIGITAL 0-13", can be used either as input or output pins. Pins that labeled with tilde ~ symbol (3,5,6,9,10,11) can act as normal digital pins, but also can be used for Pulse-Width Modulation (PWM), which simulates analog output such as fading an LED in and out.

<!-- class = "animated rollIn" style = "animation-delay: 3s; color: orange" -->
Reset Switch: used to reset the microcontroller. this can be very useful if your code doesn't repeat, and you want to test it multiple times.

<!-- class = "animated rollIn" style = "animation-delay: 3s; color: blue" -->
Crystal Oscillator: On each tick, the microcontroller performs one operation, and it ticks 16 million times in one second.

<!-- class = "animated rollIn" style = "animation-delay: 3s; color: brown" -->
TX RX Indicator: TX stands for transmit, and RX for receive. They blinking whenever the UNO board is transmitting or receiving data.



#### Power Supply
<br/>

There are some ways for powered the Arduino:
1. Battery. <br/>
<br/>
2. AC/DC adapter, which provide an output of 9V and 1A.<br/>
<br/>
3. USB Connecter.<br/>
<br/>
4. 5V pin.<br/>
<br/>
![image example](pic/ac.jpeg)
![image example](pic/usb.jpg)
![image example](pic/power.jpg)


#### Breadboard
<br/>
**What is the breadboard?**
Breadboard helps building electronic circuits without soldering any components together, it used to make the necessary connections between individual components. 
#### Sensors
## Programming the Arduino
#### The IDE Interface
#### Libraries

## Arduino Code

## Component and Tool Guide

## Learning by Example
