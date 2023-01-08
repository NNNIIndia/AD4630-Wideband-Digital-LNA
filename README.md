# AD4630 Wideband Digital LNA
## Introduction
[under construction]
## Project Motivation
### Goals:
- Wideband sampling and digitally filtering samples to desired bandwidth
- Ultralow 1/f corner front end with AC and DC paths for noise and nanovolt measurements (TBD)
- Optically isolated digital and analog sections: This is achieved easiest using a separate controller for front-end side, and using something like a UART isolator and a UART-USB bridge on the other side. 
- Battery powered (front end at least, digital section USB powered): This one might be a bit challenging, for example, what kind of batteries will be used? What voltages to power the front end with? Single ended or bipolar?
### Challenges: 
- Sample storage and processing
- Evaluating noise performance
- Implementing optical isolation and battery power
- Input analog circuitry to accomodate differential output and AC coupled input
## Usage
[under construction]
## List of Files
- Hardware: KiCAD PCB files.
![Prototype PCB layout](https://github.com/NNNILabs/AD4630-Wideband-Digital-LNA/blob/main/resources/front.PNG)
- Software: [under construction]
  - Simulation: LTspice .asc file.
## Application Examples
[under construction]
- The LNA outputs raw samples that can be stored in a .csv file and interpreted by an [NSD](https://github.com/macaba/NSD) program. 
## Notes
- AD4630 is pin-compatible with the AD4030, which opens up some interesting possibilities in the future.
### Choice of Parts:
- AD4630 2Msps 24-bit ADC: 6.5-digit capable, fast sampling, internal filtering
- ADA4528 auto-zero op-amp: Lowest measured 1/f corner frequency
## Links
- https://github.com/macaba/NSD
- https://github.com/macaba/ad4630-pico-breakout
- https://github.com/macaba/Nuts/blob/main/images/NSD.png
- https://www.analog.com/media/en/technical-documentation/data-sheets/ad4630-24_ad4632-24.pdf
