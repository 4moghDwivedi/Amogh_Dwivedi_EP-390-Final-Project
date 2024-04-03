# EP-390 Final Project
 "Amogh's first and final instrument during his studies at Berklee College of Music in Boston, Massachusetts!"


## Proposal

#### Likely name
 Amogh’s first and final instrument during his studies at Berklee College of Music in Boston Massachusetts!

#### Basic design
At the core of my instrument will be a temperature sensor which will affect the general mood of the piece. For instance, on a rainy day, it could make the music sound happier, and lazy on a sunny day (my personal response to these weathers). The weather in other words, ‘initialises’ the composition’s base state and variables, like tempo, instrument choice, available pool of choices for pitches, rhythms, etc.

I admit that I am somewhat reluctant to implement human gestures but it might be appropriate to implement a few gestures that my classmates presented, such as force sensitive resistors, and ultrasonic sensors. This in my view would be the secondary portion of my composition, where interactions by user can trigger additional instruments/sound objects. Note that the general quality of these would have already been affected by the weather FIRST.

#### Good outcome deliverable

* Good implementation with MAX for the temperature sensor
* A clear spectrum of musical choices that correspond to temperature
* Acceptable implementation of force sensitive resistors and ultrasonic sensors

#### Better outcome deliverable
* Stronger musical range and expression with MAX that is more detailed, such as by randomising between options within a range. (Ex. There are
three possible modes within a temp range of 10-15 degrees celsius and the choice is arbitrarily picked). Additionally time of day can also affect the 	general mood)
* Additional humidity data processing
* More precise processing of incoming data from force resistive/ultrasonic sensors based on weather
	
#### Best outcome deliverable
* The instrument can be placed outdoors and can operate on batteries only, and no laptop
use multiple speakers within a large structure (like a superhero or something similar) that might be placed in the Esplanade or somewhere similar
* the composition is fit to run for an extended period of time, such as a week.

##### Next Steps
I certainly need to purchase a temperature sensor. Since I have been spending plenty of time coding generative music in Max as of late, coding the music should not be an unfamiliar challenge. I have never really worked with hardware sincerely, so being able to process the incoming data in a way which reproduces accessible musical results will be an important discovery (for instance, I wouldn’t want the minor fluctuations in the temperature to drastically change the musical output). 	
    
    
    
Processing the incoming data from the force sensitive resistors/ultrasonic sensors will also be important. I don’t want those objects to work trigger samples at 100% amplitude every time. The music should sound organic and I would like to implement a system where spamming the sensors with data is not musically rewarding. That will naturally discourage unmusicality but will also be a cool technical feat!

