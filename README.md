## First version

This is the first version of the laser engraver. For this version, I used an Arduino with the [GRBL](https://github.com/grbl/grbl) firmware as the brains of the unit. I used the trays from optical drives for X and Y axis movement since they have stepper motors. In addition to the stepper motors, the laser diodes used in optical drives can also be used but they are difficult to remove intact. 

I used a 15 watt laser diode and it required 12 volts, however, the Arduino could only handle 5 volts. I used a modified pc power supply to provide the differenet voltages and used a relay to swtich the laser on/off.


![Image 1](assets/image1.jpg)
![Image 2](assets/image2.jpg)
![Gif 1](assets/gif1.gif)
![Gif 2](assets/gif2.gif)

## Second Version

For this version, I refurbished a 3D printer. I used a [RAMBO](https://reprap.org/wiki/Rambo) mother board with [Marlin](https://marlinfw.org/) fimrware. This is actually a 3D printer firmware but it has support for laser engraving since the Gcodes for the two are very similar. 

One of the main reasons that I decided to make a second version was because I was having problems switching the laser on/off. The pin that controlled the laser on the arduino was next to limit switch pins. In some cases, when the laser was turned on/off and the relay switched, it would cause feedback which would trigger the limit switch pins next to it. The Rambo board I used also took 12 volts so I didnt have to use a relay to turn it on/off. 

I was also having problems with the small stepper motors I was using. They were small and not designed to carry the load I was putting them under for the ammount of time they were running for so they would get bery hot and start melting things. 

![Image 3](assets/image3.jpg)
![Image 4](assets/image4.jpg)
