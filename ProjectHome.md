# Open-NGDI - Open Next-Gen Digital Interface #

### Intro ###
> This project is for the DIY audiophile, the Ham, the pioneering researcher, the scientist, and anyone else in need of a high quality digital interface to the physical world. Current plans are to develop an interface capable of capturing the "RAW" data stream from today's high dynamic range analog to digital converters, operating internally with an "Multi-bit Delta-Sigma, AKA Sigma-DPCM" Architecture.

### License ###
> This is a hardware project with required software needed in the development. This creates an interesting licensing situation. All software and it's documentation will fall under the GPL v2, while the hardware and it's documentation require another license. All software and hardware will be open source, including all documentation, which includes PCB layouts, FPGA code, Gerber files, etc.

An open hardware license has not been chosen yet, but currently leaning towards the [Open-source Hardware License Draft Definition 1.0](http://freedomdefined.org/OSHW). Other options include the [LGPL](http://www.gnu.org/copyleft/lesser.html) for VHDL code as recommended by [OpenCORES](http://www.opencores.org/), the [TAPR OHL v1.2](http://www.tapr.org/ohl.html), the [CERN OHL V1.2](http://www.ohwr.org/documents/88), and [others](http://www.inmojo.com/licenses/).

Repository for Source code will be either [Google Code](http://code.google.com/), or [Sourceforge](http://www.sourceforge.net/). A Hardware Repository has not been chosen yet. The [CERN Open Hardware Repository](http://www.ohwr.org) is a likely candidate, but would require use of either the TAPR OHL or CERN OHL.

### Software ###
> There is some necessary software that will be developed. Most important will be a cross-platform driver and basic software to record/playback data. Software for sample rate conversion, and DAW software for multi-track recording will be developed as well, in addition to software developed for SDR by the Open-NGSDR project.

### Hardware ###
PRELIMINARY LIST OF OPTIONS:
  * FPGA will need to support Data rate anticipated. (See; [Bitrate Comparison Doc.](http://code.google.com/p/open-ngdi/downloads/detail?name=Bitrate%20Comparison.pdf))
  * [WhiteRabbit](http://www.ohwr.org/projects/white-rabbit) project is very promising. It allows synched packets from multiple nodes, separated by as much as 10km with ethernet over Copper or Fibre. Sub Nanosecond timing sync between nodes, high bandwidth, already a complete IP Core, could be programmed to an FPGA, plus it's an Open Standard. Would require use of [CERN OHL v1.2](http://www.ohwr.org/documents/88). Supports similar ADC's and DAC's. Might be too expensive for general use, but could make simple switching equipment specifically for this project.
  * PCB will need design/testing. RF Frequencies will need taming, and creates a necessity for very clean layout and great care in design. Testing will be done to verify a certain level of functionality.

### Sister Project ###
> The Main sister project of the OpenNGDI is the [OpenNGSDR](http://code.google.com/p/open-ngsdr), a branch specifically for Software defined radio and measurement purposes. It will contain certain hardware extensions not required for general use. All analog stages and ADC/DAC hardware will be external, modular and endlessly configurable.

### Child Projects ###
> The main sister projects will be named [OpenNGADC](http://code.google.com/p/open-ngadc/) & [OpenNGDAC](http://code.google.com/p/open-ngdac/), there main goals will be to develop external pcb's after choosing an appropriate commercial ADC and DAC. (It is well beyond the scope of these projects to have an ADC or DAC IC fabricated.) This is less critical as alternatives exist for testing, making these projects secondary to the main goals of this project. The scope of this project is intentionally large to cover as many bases as possible, with the hope of increasing help in the critical stages of development.

### Community ###
> No major technical decisions have been made, except minimum sample rates. I hope to make the process very democratic, hopefully giving this project a good opportunity of getting off the ground.


> This project has high goals, but I strongly believe they are attainable. This project has many uses crossing the board, and I hope will find itself used in many other projects. Only by upping the bar for open-source development will we help spur new generations of technology for public use and education. The developing world and scientists alike will be helped by lowered entry costs into cutting edge research and technology. Though many of the tasks described are within the capability of common USB logic analyzers, this project aims to refine this functionality to the same level afforded to more common formats.

### Project Status ###

  * 2011.9 - Paper "Theoretical New Formats" written
  * 2011.12 - Definition Stage