---
layout: page
title: CNC_Plotter
description: 2D image plotter
img: assets/img/cnc.png
importance: 6
category: <
---
### <a href="https://github.com/ChinChinati/CNC_Plotter">[code]</a>
# CNC Plotter - Image Drawing Project

This GitHub repository contains the complete code and resources for building a **CNC Plotter** that can draw any image on paper. The plotter is based on an **Arduino Uno** board and utilizes **stepper motors** to precisely control the movement of the drawing mechanism. The project also employs a **servo motor** to control the pen holder, allowing for high-precision image drawing on a piece of paper. 

The CNC Plotter can take any image file, convert it into a series of movement instructions (G-code), and then draw it onto paper. This project is ideal for makers, hobbyists, and students interested in CNC machining, robotics, or image processing, as it uses commonly available hardware components and open-source software tools.

---
<iframe width="930" height="450" src="https://www.youtube.com/embed/TETPuLBlouc?si=v8t3RjRyj8mQDe08" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
---

## Project Overview

The CNC Plotter uses a **two-axis setup** to move the pen holder across the surface of the paper. The system relies on precise control of the stepper motors to achieve the accuracy needed for drawing complex images or patterns.

---

## How the Project Was Made

### Hardware Components

The following hardware components were used to build the CNC Plotter:

- **Arduino Uno Board**: Acts as the brain of the CNC plotter, receiving commands and controlling the motors.
- **2 x DVD Stepper Motors**: These motors control the movement of the plotter along the X and Y axes, allowing for precise control of the pen's position.
- **1 x Servo Motor**: Controls the pen holder's vertical movement, allowing it to lift and lower the pen for drawing.
- **5V Power Supply**: Powers the Arduino board and motors, ensuring a stable power source for the operation.
- **L Joints**: Used to construct the frame of the CNC plotter and provide structural support.
- **2 x L293N Motor Driver**: These motor drivers control the stepper motors by receiving signals from the Arduino and powering the motors.
- **Pen Holder**: Holds the pen in place and is attached to the servo motor, allowing for precise vertical movement.
- **Aluminum Composite Sheets**: Used to create the frame of the plotter. This material provides a strong and lightweight structure.
- **Cardboard Sheet**: Serves as the drawing surface where the plotter will draw the images.

The CNC plotter's frame is made from **Aluminum Composite Sheets**, which provide stability and support for the motors and other components. The **stepper motors** are mounted on the frame using **L joints**, while the **servo motor** is mounted to a separate frame to control the pen holder's vertical motion.

The stepper motors are connected to the **L293N motor drivers**, which interface with the **Arduino Uno** to control their movement. The **servo motor** adjusts the pen holder’s height, enabling the pen to be lifted when moving between drawing points and lowered to the drawing surface when making marks.

---

### Software Components

The CNC Plotter relies on several open-source software components for both the design and control of the machine:

- **Arduino IDE**: Used to write the code for controlling the Arduino board. The code interprets movement instructions and sends signals to the motors to move the plotter's head.
- **Processing3**: A graphical tool used for generating G-code commands from image files. It acts as a bridge between the image design and the plotter, sending the commands to the Arduino.
- **Inkscape**: A popular vector graphics editor used for preparing images and converting them into G-code. Inkscape can export the design in **DXF** format, which is then converted into **G-code** commands using an extension.

### How the System Works

1. **Image Preparation**:
   - The first step in the process is converting the image to a vector format that can be understood by the CNC plotter. This is done by exporting the image as a **DXF** file using Inkscape. DXF is a common format used in CNC machines that describes vector graphics.
   
2. **Converting DXF to G-code**:
   - In Inkscape, the **DXF** file is loaded and then converted into **G-code** commands using an Inkscape extension. G-code is a language that CNC machines understand, which dictates the movement of the plotter’s motors.

3. **Sending G-code to the Plotter**:
   - The G-code commands are saved as a **text file** and loaded into **Processing3**. The Processing script reads the G-code file and sends commands to the Arduino. These commands control the stepper motors and servo motor to move the pen holder and trace the design onto the paper.

4. **Drawing on Paper**:
   - The CNC Plotter, guided by the G-code, moves the pen holder over the surface of the paper, drawing the image by making precise pen marks. The **servo motor** controls whether the pen is in the up (non-drawing) or down (drawing) position, ensuring that the pen only touches the paper when needed.

---

## Project Design and Workflow

The design of the CNC plotter is modular and scalable. The key steps in the process are:

1. **Setting up the hardware**: 
   - Assemble the frame using **L joints** and **aluminum composite sheets** to support the stepper motors and servo motor.
   - Attach the **stepper motors** to the frame and connect them to the **L293N motor drivers**.
   - Connect the **servo motor** to the pen holder, and attach the pen holder mechanism to the motor.
   - Mount the **Arduino Uno** on the frame and wire it up to control all motors.

2. **Software setup**: 
   - Write and upload the code to the **Arduino** using the **Arduino IDE**. The code will control the stepper motors based on incoming G-code.
   - Use **Inkscape** to convert an image into **G-code**, then send it to the Arduino via **Processing3**.

3. **Drawing**: 
   - Place a **cardboard sheet** on the drawing surface.
   - Begin the drawing by sending the G-code to the plotter, and watch as the pen moves to recreate the image on the paper.
