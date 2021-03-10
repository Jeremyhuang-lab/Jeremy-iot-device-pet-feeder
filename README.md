# Jeremy-iot-device-pet-feeder
This project is developed using Tuya SDK, which enables you to quickly develop branded apps connecting and controlling smart scenarios of many devices.       
For more information, please check Tuya Developer Website.

1.Product name
==
Smart Pet feeder

2.Product creative reasons
==
Clothes are designed to resist the cold, and then they are given more connotations.
Fire is used for heating and deterring beasts before it is used for energy.
Tools are for better product acquisition, and then they evolve into machines.
The evolution of human civilization is not laziness, but human beings have been pursuing their own comfort.

With people’s increasing material life needs and yearning for a better life, many people of all walks of life and all ages have begun to raise pets, but contemporary workers usually work at 007, and they really don’t have time to take care of their pets. In the last year of the epidemic, many people were unable to feed their pets at work due to the lockdown of the city. Therefore, smart pet feeders came into being.


3.Product Features
==
APP control Timing and quantification Automatic grain feeding Scientific feeding plan Food shortage reminder Intelligent water feeding Anhydrous detection Environmental monitoring Voice control Real-time video monitoring (to be developed)

APP control: Cooperate with Tuya WIFI module through Tuya Smart APP, transplant related SDK, and use the official debugging assistant to test the function

Timing and quantification Through the timer of the single-chip microcomputer, the motor is enabled to rotate every 6 hours to open the grain outlet for 2 seconds. After 2 seconds, the motor reverses and the grain outlet closes.

Automatic grain output, APP sets the time, and sends instructions to control the single-chip microcomputer to output grain at the corresponding time.

Scientific feeding plan, when customers go out for a long time, set the intelligent feeding mode, the program automatically sets the feeding plan, and puts it regularly.

For intelligent water feeding, the mold can be set as a grain outlet and a drain outlet, which are separately controlled by two motors, and the corresponding hatch is opened for delivery.

Anhydrous detection The water can be detected by dry reed pipe or iron sheet. The principle is to detect the voltage change of the iron sheet when there is water or lack of water, and the single-chip ADC is used to detect.

Environmental monitoring Add a temperature and humidity sensor, when the temperature is too high, immediately open the drain, drink water for the pet, and change the corresponding feeding plan.

Voice control, through the Tuya WIFI module docking smart voice such as Xiaodu, voice feeding.


Real-time video monitoring is expected to be possible through OPENCV or whether it can be connected to other video equipment through Tuya WIFI module, and send real-time video of pets through them.

4.Part of the design rules
==
Single-chip main control select domestic 8051 single-chip STC15W58S4 or select STM32F103 series

Motor drive adopts H-bridge drive. Single-chip PWM control of brushed DC motor speed or ULN2003 to drive unipolar stepping motor also uses single-chip PWM to control direction and speed.

Temperature and humidity chip can choose SHT30 or DHT11

RGB lighting effects can be added at the same time

If possible, use a 3.3V boost 5V chip to drive the UVC lamp to disinfect food and drinking water regularly.

5. Development plan
==
1) Prepare materials before March 25
2) Embedded development and cloud development from March 25 to April 15
3) Overall commissioning before April 20.


