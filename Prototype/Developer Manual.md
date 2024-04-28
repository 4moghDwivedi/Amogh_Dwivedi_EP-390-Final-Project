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