# 1. Introduction to the Arduino Uno R3
The Arduino Uno R3 is a microcontroller development board designed by Arduino with which we can controll various components. It is a small and compact microcontroller that has 6 analog pins, 14 digital pins, 5V and 3.3V output pins, reset button and reset pin and more. In this article I will be discussing the ins and outs of the Arduino Uno R3 and its capabilities to document the features and serve as a reference for future projects. It is one of the most popular and widely used microcontroller boards for various reasons. It is beginner friendly, easy to use, has a big following and community support and lots of libraries. For these reasons, the Arduino Uno R3 is a must have for beginners.

# 2 Technical Specifications
The Arduino Uno has the **ATMega328P** and the **ATMega16U2** microcontrollers which have a multitude of features that will be discussed further in this section. Both microcontrollers run on a 5V AVR 8-bit architecture. The **ATMega328P** clocks at up to 16 MHz.
<img width="961" height="584" alt="image" src="https://github.com/user-attachments/assets/16d5ae50-e7b2-42b7-ae0a-cf3a8efc6f51" />
## 2.1 Memory
The Arduino Uno R3 has **2** processors, namely:
  - The **ATMega328P** (main processor, this is where you upload your code to) which has 32 kB of flash, 2 kB SRAM and 1 kB EEPROM memory and is easily accessible.
  - The **ATMega16U2** (this is where the firmware is stored) which has 16 kB of flash, 512 B SRAM and 512 B of EEPROM memory and is not easily accessible.
We will focus on the **ATMega328P** characteristics.
### 2.1.1 Flash memory
Flash memory is a storage medium that is non-volatile, which means that after power is cut off it **does not** erase itself. You can overwrite it or reset it completely. The **ATMega328P** has 32 kB of flash memory so you can upload code into it to execute tasks. A small part of the flash memory is dedicated to the bootloader[^1]. The main function of the bootloader is to receive data from the **ATMega16U2** and to write it into the **ATMega328P**'s flash memory.
### 2.1.2 SRAM
Static Random Access Memory, SRAM, is a volatile storage medium. It will hold on to its data as long as power is connected. Data can be accessed, read or written, randomly like any other RAM memories. For example:
```
#define LED_D2 2
int counter = 0;
```
Here ```#define LED_D2 2``` will not be stored in the SRAM because it **is not** a variable[^2] while ```int counter = 0``` is a **variable** and will be stored in the SRAM. Some variable may or may not be stored in the SRAM, but this is out of the scope of this article.
### 2.1.3 EEPROM
Electrically Erasable Programmable Read-Only memory is a non-volatile storage medium. It stores data byte by byte and is easily accessible on the Arduino IDE with the EEPROM library ```#include <EEPROM.h>```. This is very useful when you need some specific data to be stored even if the Arduino is powered off. 


# 3. The pinouts 
The arduino Uno R3 has a multidude of pins each with its own characteristics and use cases. In the image below we can see the pinouts.
<img width="1038" height="811" alt="image" src="https://github.com/user-attachments/assets/9beb0756-e2ce-4b1d-b68e-8f9193820f2b" />

>The Arduino Uno R3 is rated to work at a minimum temperature of -40 C and at a maximum temperature fo 85 C (it is mentioned that at these extreme temperatures some components might not work).





# Sources
1. https://en.wikipedia.org/wiki/Flash_memory
2. https://en.wikipedia.org/wiki/Static_random-access_memory
3. https://cplusplus.com/doc/tutorial/preprocessor/
4. https://docs.arduino.cc/learn/built-in-libraries/eeprom/


[^1]: 0.5 kB is not accessible and reserved for the bootloader
[^2]: ```#define``` is a preprocessing macro (3)
