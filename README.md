# Dynamometer_HSWET
All files pertaining to the Dynamometer Operation (particular to use by HSWET)

# Common Problems that I've encountered

Dynamometer not connecting to computer while using odrivetool

  S: I'd either power cycle the dynamometer, ensure the dynamometer is in RUN mode (the physical switch on the dynamometer), and if all else fails reflash the odrivetool with the latest firmware available on the official ODrive git.

Followup: The dynamometer is a pain to flash what do?

  S: Use STM32CubeProgrammer, if HSWET doesn't have a committed account then make one yourself, it's free. Instructions on how to flash the odrivetool with this program can be found here -- https://docs.odriverobotics.com/v/latest/odrivetool.html#firmware-update

Literally nothing is happening when I try to do things with Anaconda Prompt...

  S1: Make sure the power supply voltage is around 24V, too low and the motor can't run. Too high and the ODrive becomes an angry teenager.
  
  S2: Set your config to all the recommended default values and try again.
  
  S3: Check the error dump and clear between each attempt at doing something. Do your best to understand what the error is trying to tell you.
  
  S4: Become religious and find something to pray to.
  
I'm getting an error on Arduino

  S: Download the test arduino file from the official ODrive git. This should be pretty similar to the one here, because it's essentially the same thing... lol. They probably updated the firmware or the odrivetool or something and some syntax changed at some point. You can choose to use theirs or just find the difference between this one and theirs. Your choice.
