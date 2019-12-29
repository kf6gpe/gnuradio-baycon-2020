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
![source: Wikipedia; https://wiki.gnuradio.org/index.php/File:Cont_to_digital.png](images/cont-to-digital.png)

# Sampling a signal - things to look out for
* Tradeoff between sample rate & computing requirements
* Tradeoff between cost, sample rate, and sample resolution
* Aliasing

# A word on sampling
* More samples mean more expensive A/D converters
* More samples means more computing power to process the samples
* Faster sampling means higher cost!

# A word on resolution
* Determines the number of discrete steps measurable in the amplitude of a signal
* Higher resolution generally means higher cost A/D
* Sometimes a lower noise lower-resolution A/D is better than a higher resolution A/D!

# Aliasing in sampling
![source: Wikipedia; https://en.wikipedia.org/wiki/Nyquist–Shannon_sampling_theorem#/media/File:CPT-sound-nyquist-thereom-1.5percycle.svg](images/pericycle.png)

# Aliasing in the frequency domain
![source: Wikpedia; https://en.wikipedia.org/wiki/Nyquist–Shannon_sampling_theorem](images/aliasing.png)

# Filtering
* Uses signal processing on the digitally sampled signal.
* Requires fast processsing for addition & multiplication
* Depending on sample rate, can create far steeper cutoffs for the same component prices

# Filtering: finite impulse response filter
![source: Wikipedia; https://en.wikipedia.org/wiki/Digital_filter](images/fir.png)

# Filtering: Infinite impulse response filter
![source: Wikipedia; https://en.wikipedia.org/wiki/Infinite_impulse_response](images/iir.png)

# Modulation
* More math!, e.g.
* AM can be accomplished multiplying the carrier by the audio signal
* BPSK can be accomplished by changing the phase of the carrier

# Demodulation
* Still more math
* Additional use of signal processing can provide symbol recovery, error detection & timing synchronization

# Block diagram of a typical SDR
![source: Wikipedia; https://commons.wikimedia.org/wiki/File:SDR_et_WF.svg](images/sdr.png)

# A word on hardware
* You need a moderately fast PC running Linux, Windows, or macOS.
* For RF experiments, you need some sort of SDR hardware
* [RTL-SDR](http://www.rtl-sdr.com) is a cheap receiver (check the raffle table!) 
* [hackRF](https://greatscottgadgets.com/hackrf/) is a popular transceiver
* [LimeSDR](https://limemicro.com/products/boards/limesdr/) is another newer transceiver platform
* Lots of other choices!

# What does GNU Radio give me?
* Over 400 DSP blocks, including filters, modulators, demodulators, visualization tools
* Flow-based construction of radios & subsystems
* The ability to add new blocks with code in Python or C++
  

# Getting GNU Radio
* On Linux, use your package manager.
* On Windows, use an installer.
* On macOS, use MacPorts.
* Did I mention that it's open source! You can also build from the source code.
* See the [GNU Radio Wiki](https://wiki.gnuradio.org/index.php/InstallingGR) for more details.
  
# GNU Radio Companion

# Modeling SDRs using flow diagrams


https://wiki.gnuradio.org/index.php/Guided_Tutorial_PSK_Demodulation




