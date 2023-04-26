# ADCSST

### 🗒️ Description:
This project aims to develop a low-cost attitude determination module for the CubeSat developed by the super team project from OBSAT - MCTI. The attitude determination and control system (ADCS) is a subsystem of a CubeSat that is responsible for determining, maintaining and correcting the orientation and position of the satellite in orbit. The ADCS consists of sensors, actuators, and algorithms that work together to measure the attitude of the CubeSat and correct it when necessary. 

### 📘 Contact information:
Name: Diego Anestor Coutinho  
Email: diego.anestor@gec.inatel.br

### ©️ Copyright statement:
In this project, every mention of the word "author" refers to [Diego Anestor Coutinho](https://www.linkedin.com/in/diego-anestor-coutinho).  
All the code in this project is the exclusive property of the author and is protected by intellectual property laws. No part of this code may be copied, modified, distributed, or licensed without the prior written consent of the author. Any unauthorized use of this code will constitute a violation of the author's rights and may result in legal action.

---
### Project overview diagram:

The project aims to design and implement a low-cost and low-power attitude determination module for a CubeSat using an MPU9250 inertial sensor and an attiny44 microcontroller. The MPU9250 sensor integrates a 3-axis gyroscope, a 3-axis accelerometer and a 3-axis magnetometer, which can measure the angular velocity, linear acceleration and magnetic field of the CubeSat. The attiny44 microcontroller communicates with the sensor via I2C protocol using a software serial interface and processes the sensor data to estimate the orientation of the CubeSat in real time. The module can provide attitude information to other subsystems of the CubeSat via the serial bus as requested. The system is supplied with 5V and GND. The supply voltage is downregulated to 2V5 and 3V3 with onboard linear regulators.

<p loat="left" >
  <img style="margin:1rem 0.5rem; width: 90%; float: left;" src="https://github.com/DIEGOVZK/ADCSST/blob/pio_devenv/documentation/sysoverview.drawio.png">
</p>