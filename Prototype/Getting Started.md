# EP-390 Final Project
 "Amogh's first and final instrument during his studies at Berklee College of Music in Boston, Massachusetts!"


## Getting Started

### Required files and packages
 * Max/MSP
* RNBO Guitar Pedals (Available in Max/MSP Package Manager)
* Adafruit SHT31 Code in Arduino IDE (Available in packages)

### Assembly
Please find attached images. The photoresistor uses analog inputs, while the temperature/humidity sensor uses I2C.

https://drive.google.com/open?id=1ZhsOiN--ntKM7ahD5AeEXbjJAWjagPvC&usp=drive_fs

### Basic setup
At this stage of my prototyping, I haven't yet combined the two pieces of Arduino codes yet. I would reccomend launching the photoresistor one as it is more likely to yield a more interesting musical output.

After the Arduino code is running and the photoresistor value is being communicated through serial, launch the Max patch. Turn on the toggle associated with the serial object, and then turn on DSP. The patch should start generating the music on its own.

Try covering the photo resistor to see the change in timbre. The temperature sensor (or its slider equivalent) will produce changes in tempo as well.