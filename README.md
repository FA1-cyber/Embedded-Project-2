# Embedded-Project-2

## How to build the project
 1.Open CubeMX and create the following configurations: 
  USART1_RX and USART1_TX are used for receiving the coordinates from the GPS module.
  USART2_RX and USART2_TX are used to transmit the coordinates to the mobile phone using the Bluetooth module.
  GPIO_Input is used to get a value from the metal sensor to check whether a metal is detected or not (1 - metal detected, 0 - no metal).
  RCC set to Crystal/Ceramic Resonator.
  SYS set to Serial Wire.
  Picture of the configuration: https://drive.google.com/file/d/1steU1Vv7ZO_chwA7Wr9h4wtD2ooD69ww/view?usp=sharing
  
2. Generate code from CubeMX
3. Copy the codes from the main.c and stm3214xx_it.c to the designted files
4. Download the program to the STM microcontroller  
5. Connect and android phone to the bluetooth module using the Serial Bluetooth Terminal Application
6. Access the LOOMO robot in Developer mode (Settings > System > Loomo Developer > Developer Mode)
7. Open Android Studio and follow these steps:
   a. Open a new and choose the "Empty Project" option
   b. Open the main java file, and copy the code "Loomo_motion.java" in the repo
   c. Open the build.gradle file to add the dependencies and copy the code in "build.gradle" in the repo
   d. Build the project
   e. Connect the LOOMO to your device using a USB-C cable and wait till Android studio detects the robot then download the code to the robot
   f. Open the program from the LOOMO having the same name of the project
   g. LOOMO is ready for your voice commands!
