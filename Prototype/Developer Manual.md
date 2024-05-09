# EP-390 Final Project
 "Amogh's first and final instrument during his studies at Berklee College of Music in Boston, Massachusetts!"


## Development Journal

### Bill of Materials
Please find the attached document. Additionally, an SHT31-D needs to be purchased.

https://www.adafruit.com/product/2857
 
### Implementation Details

This work centers around a generative composition. The composition interacts with the environment and the musical parameters of the composition are affected accordingly. So far, temperature and amount of light are the parameters that are controlling the composition. Additionally, I plan on incorporating humidity, water level, and ultrasonic data to help make the composition more unique.

From the start, I imagined the composition taking place in the Charles River Esplanade in Boston, and wanted it to be placed somewhere along the walking paths. The area is quite well exposed to the elements, and temperature/light data is really easy to capture. I was also inspired by John Cage's "As Long As Possible", and that gave me some courage to pursue the idea of a composition that would run for 1 year. Throughout the year, as the weather changes, the recurring 'users' of the esplanade would be able to notice changes to the music due to the nature of the instrument.

My general experience of the esplanade is marked by walking past things, and not really interacting with too many things, and most walkers and joggers would naturally agree. Therfore, sensors that would capture data from the environment as opposed to humans was more appropriate. Understandably, some people would be curious and try to investigate the musical instrument, which is why I plan on incorporating an ultrasonic sensor.

The instrument shows promise. The music sounds accessible and appropriate for commoners (i.e. not music snobs at music school), and the interaction between the music sounds, and the nature sounds of the esplanade, would combine well. The music sounds fairly organic and the timbres are okay, and the current implementation of the photoresistor and temperature sensor is functional.

However, much work remains to be done. I need to code the music associated with summer (which is likely to be an FM oriented atonal piece). The music can also use more pause and breath as listening to the piece for one year can be quite exhausting if it is busy. Further implementation of other sensors is yet to be done, and I look forward to accomplishing these challenges soon.

### Hardware assembly
Please find attached image. Note: 2k resistor.

https://drive.google.com/open?id=1ZhsOiN--ntKM7ahD5AeEXbjJAWjagPvC&usp=drive_fs

## Final Deliverable Updates

Most of my coding work was done in Arduino IDE, where I switched from a delay() approach to a millis() approach. This was a bit of a learning curve but there are helpful online tutorials which made the implementation not too difficult. I also implemented rolling averages, in order to yield more meaningful data. The sensors are fairly sensitive and the rolling averages seem to help in ignoring noisy data. However, the communication rate between the Teensy and Max still seems somewhat subpar, despite lowering the polling rates. An interesting solution I stumbled upon was having two seperate 'structs' for all sensors for firstly raw measurement data, and secondly the methods that would print rolling averages of said data, as the 'polling' rates for both were different. This solution was generated solely because of the unique intersection between using the millis() approach, and implementing rolling averages, and it was a pleasant discovery.

Incorporated humidity data, which affects the vibrato depth of various instruments. The ultrasonic sensor fades in or fades out different instrument and also results in some timbral changes.

Changed metro rates of various instrument groups. Upon receiving peer and instructor feedback, I decided to make the composition way sparser, as the sounds of the environment could then be considered a part of the composition. A constant composition would certainly get annoying to listen to. These rates could still be easilly changed to longer durations in case of an actual outdoors installation.

Added presentation mode for the expo presentation, which clearly demonstrated the raw measurement of the various sensors. Unfortunately, due to the generative aspect of the composition, I often had to awkwardly wait for the composition to start running in order to demonstrate how the music responded to the different sensors, and so I somewhat haphazardly added the button for the 'winter' bass so trigger it manually. Further considerations like these can be taken in order to make presentations smoother. 

An issue I encountered was not being able to smoothly transition between the summer and winter weather I had programmed. My solution was to fade out the different instruments of the two sections at different thresholds. In other words, the bass instruments, for instnance, of both seasons might overlap. The chords of the winter season may fade out sooner than the bass part associated with the same season, which made the 'intermediate' season possible to realize.

