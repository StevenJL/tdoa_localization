## Time Delay of Arrival Localization

### Background Info

I wrote this code when I was working as a signals processing researcher at SF State University.  I get an email once a while asking about this algorithm so I'm making a github repo with better documentation around it.  Please read this before emailing me.

### FAQ

#### What is TDOA Localization?

I wrote an [expository paper about it here](https://s3-us-west-1.amazonaws.com/stevenjl-bucket/tdoa_localization.pdf).

#### What does your program do exactly?

It's a proof-of-concept of demonstration of how TDOA works.  I randomly generate a location inside a microphone array and simulate the signals recieved by these microphones adjusting for spherical attenuation and time delay of arrival.  This algorithm attempts to locate the source of the signal using the TDOA Localization technique described above.

#### What does this graph mean?

![alt tdoa_trials](https://s3-us-west-1.amazonaws.com/stevenjl-bucket/TDOA_20trials.jpg)

It means I simulated 20 random locations and attempted to locate them with the TDOA Localization algorithm and plotted the actual position and the estimated position.  As you can tell, this algorithm really works.  Note the scale on the x and y axis are in meters.


#### Where is the sample.wav file?

It can be any wav file that is mostly silence with a few bursts.  The best case is a recording of a gunshot (mostly silent with a big burst).  The worse case would be a recording of white noise throughout.

My sample.wav example consists of a crow going 'caw caw'.
