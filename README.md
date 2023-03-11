## ISS-overhead
If you don't know what ISS means, I've extracted the clarification from https://www.nasa.gov:
> __The International Space Station(ISS) is a large spacecraft in orbit around Earth. It serves as a home where crews of astronauts and cosmonauts live. The space station is also a unique science laboratory. Several nations worked together to build and use the space station. The space station is made of parts that were assembled in space by astronauts.__ 

Cool fact:  
>__It is the third brightest object in the sky and easy to spot if you know when to look up. Visible to the naked eye, it looks like a fast-moving plane only much higher and traveling thousands of miles an hour faster!__  

This project was designed to be a notifier by sending an email when the ISS is above, in the sky, and visible (i.e. it is night). For this, I found out the latitude and longitude of my location, and these were given as API parameters to find out what time the sun rises and sets in a 24-hour format. 
The other important aspect is to find out the latitude and longitude of the ISS and establishing whether it is in my vicinity, with a margin of error of -5 and +5. To get this data, I made a request to the specific api and formatted it as needed.    

__If both conditions are met, an email notification will be sent to my email address.__
