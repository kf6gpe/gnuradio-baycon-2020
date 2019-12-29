% SDR with GNU Radio
% Ray Rischpater, KF6GPE kf6gpe@arrl.net | kf6gpe.org  
% BayCon 2020, 8 February 2019

# What we're talking about today
* What's GNU Radio?
* A very basic introduction to SDR
* A word on hardware
* Getting GNU Radio
* GNU Radio Companion
* Writing 



# What's GNU Radio?
* Free & open source software
* Provides signal-processing blocks to build software-defined radios
* Works with readily available hardware
* Runs on Linux (best), Windows and macOS
* Used in hobby and commercial applications

# A very basic introduction to SDR
* Uses digital representations of signals 
* Uses lots of math to implement things like modulation & filters

# Sampling a signal
* Analog signals sampled periodically
* Sample rates should be at least 2x maximum frequency rate (Nyquist theorem)

# Sampling a signal
![source: https://wiki.gnuradio.org/index.php/File:Cont_to_digital.png](images/cont-to-digital.png)

# Sampling a signal - things to watch out for
* Tradeoff between sample rate & computing requirements
* Tradeoff between cost, sample rate, and sample resolution
* Aliasing

# A word on sample rates
* More samples mean more expensive A/D converters
* More samples means more computing power to process the samples
* Faster sampling means higher cost!

# A word on resolution
* Determines the number of discrete steps measurable in the amplitude of a signal
* Higher resolution generally means higher cost A/D
* Sometimes a low noise lower-resolution A/D is better than a higher resolution A/D!

# Aliasing in sampling
![source: https://en.wikipedia.org/wiki/Nyquist–Shannon_sampling_theorem#/media/File:CPT-sound-nyquist-thereom-1.5percycle.svg](images/pericycle.png)

# Aliasing in the frequency domain
![source: https://en.wikipedia.org/wiki/Nyquist–Shannon_sampling_theorem](images/aliasing.png)

# Block diagram of a typical SDR

# A word on hardware
# Getting GNU Radio
# GNU Radio Companion
# Modeling SDRs using flow diagrams




