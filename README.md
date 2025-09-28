# 1. Introduction to the Arduino Uno R3
The Arduino Uno R3 is a microcontroller development board designed by Arduino with which we can controll various components. It is a small and compact microcontroller that has 6 analog pins, 14 digital pins, 5V and 3.3V output pins, reset button and reset pin and more. In this article I will be discussing the ins and outs of the Arduino Uno R3 and its capabilities to document the features and serve as a reference for future projects. It is one of the most popular and widely used microcontroller boards for various reasons. It is beginner friendly, easy to use, has a big following and community support and lots of libraries. For these reasons, the Arduino Uno R3 is a must have for beginners.
# 2 Technical Specifications
The Arduino Uno has the **AtMega328P** and the **ATMega16U2** CPU which have a multitude of features that will be discussed furthur in this section. Both CPU runs on a 5V AVR 8-bit architecture. The **ATMega328P** clocks at up to 16 MHz.
<img width="961" height="584" alt="image" src="https://github.com/user-attachments/assets/16d5ae50-e7b2-42b7-ae0a-cf3a8efc6f51" />
## 2.1 Memory
The Arduino Uno R3 has **2** processors, namely:
  - The **ATMega328P** (main processor, this is where you upload your code to) which has 32 kB of flash, 2 kB SRAM and 1 kB EEPROM memory and is easily accessible.
  - The **ATMega16U2** (this is where the firmware is stored) which has 16 kB of flash, 512 B SRAM and 512 B of EEPROM memory and is not easily accessible.
We will focus on the **ATMega328P** characteristics.
### 2.1.1 Flash memory
Flash memory is a storage medium that is non-volatile, which means that after power is cut off it **does not** erase itself. You can overwrite it or reset it completely[^1], but not via powering it off. The **ATMega328P** has 32 kB of flash memory so you can upload code into it to execute tasks.
### 2.1.2 SRAM

### 2.1.3 EEPROM



# 3. The pinouts 
The arduino Uno R3 has a multidude of pins each with its own characteristics and use cases. In the image below we can see the pinouts.
<img width="1038" height="811" alt="image" src="https://github.com/user-attachments/assets/9beb0756-e2ce-4b1d-b68e-8f9193820f2b" />

>The Arduino Uno R3 is rated to work at a minimum temperature of -40 C and at a maximum temperature fo 85 C (it is mentioned that at these extreme temperatures some components might not work).





# Sources
https://en.wikipedia.org/wiki/Flash_memory



[^1]: 0.5 kB is not accessible and reserved for the bootloader
