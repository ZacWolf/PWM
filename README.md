# PWM.h

v 5.0.1

Created by Sam Knight
Fork by Zac Morris (@ZacWolf) zac@zacwolf.com

Modify PWM frequency on AVR (arduino) platform

Modified by Zac Morris 11/24/2018:
  1) Modified BTimerDefs.cpp to add an IF/THEN the 
  #define UINT16_MAX 65535
  #define UINT8_MAX 255

  Since those are now defined in the stdlib, and were  throwing warning messages during compile.

  Changed to:
  #ifndef UINT16_MAX
  #define UINT16_MAX 65535
  #endif
  #ifndef UINT8_MAX
  #define UINT8_MAX 255
  #endif


Modified by Terry Myers:

1. Modified examples to be in their own folders
2. Corrected a line feed character in two of the libraries so that visual studio would not error when opening them
3. Added README.MD, library.properties, and library.json files to better "integrate" to IDEs espencially Arduino IDE for begginers
4. Added new example for high resolution control of an LED
5. Added "{ 0, 0, 0, 0, 0 }, //TIMER1C" to line 107 in ATimerDefs.cpp as suggested by texmit from arduino forms

Original repository
https://code.google.com/archive/p/arduino-pwm-frequency-library/downloads

Original Arduino Forum library post by Runnerup (Sam Knight):
https://forum.arduino.cc/index.php?topic=117425.0
