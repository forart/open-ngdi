# Criteria #

Current Minimum Specifications:

  * Support up to 1.5Mhz PCM formats I/O via I2S (IIS)
  * Support Delta Sigma 1-bit up to 24.576Mhz (512fs) I/O via I2S
  * Support Delta Sigma 5-bit & 6-bit formats up to 24.576Mhz (512fs) I/O (needs to support current TOTL commercial ADC's eg. TI PCM4222, Arda AT1201, etc.)
  * Designed with an expandable modular architecture which should allow future modifications/expansion (eg. an SDR might want as high as 1+gs/s sample rate)
  * Support a modern highspeed low latency interface, probably either USB 3.0 or gigabit Ethernet (want suggestions, firewire is dead in the water, Ethernet might increase prototype cost dramatically)
  * Support many channels in software/hardware. Requires ability to gang together boards (ability to lock clocks, driver supporting 2 or more interfaces attached to one computer would be ideal, eg. the USBPAL supports 3+ boards daisy chained for 24+ channels)
  * Preferably onboard discrete clocks. Multiples of 44.1Khz and 48Khz would be optimal for audio, whether for DSD or PCM. (Possibly 1 ultra low noise SC-cut 100Mhz crystal oscillator like a Wenzel or other astronomy class oscillator, would require DDS like AD9910 or AD9912 and supporting hardware, but increases flexibility)
  * Independent isolated supplies for all components onboard, DC input (maybe super-regulators on daughter-boards, allows experimentation/upgrading)
  * Star Grounding Scheme between all modules. A low noise ground is very important for design, must not have ground loops at all frequencies to be handled. PCB design will need to be designed for RF, with great attention to ground inductance.
  * Overall modular approach (All supplies by-passable, anything ancillary can be disabled)
  * All analog stages I/O external, similar to Buffalo-II (allows easily customizing analog stages for any application, eg. the Nagra IV-SJ preamp, transformers, discrete, opamps, passive LC, or tubes)
  * Tested and documented specifications of ACTUAL hardware, as simple as it seems most projects, commercial or opensource lack this kind of testing or specification.
  * USB will allow using the standard USB Audio 1.0 and 2.0 driver models, which would simplify use for 192Khz and lower sample rates (secondary goal, this project focuses on unavailable formats.) 400Khz PCM can be supported in windows via an ASIO 2.1 driver, but will need a driver for unix and OS X. DSD will require developing a driver model to support it for Unix, OS X and Windows (maybe some hope for a standard DSD driver is on the horizon.) Hopefully a standard cross-platform open source driver model can be developed for DXD, Delta Sigma Single and Multi-bit formats. Creating a standard cross-platform driver model for Delta sigma would be very beneficial to the open source community.
  * File Format for Uncompressed Multibit Delta-Sigma will need developing. Also of great interest is developing a Lossless compression scheme and file format for Single and Multi-bit Delta-Sigma Audio. I will make a sister project, a standard will be decided and require full documentation and sample code. Possibly FLAC can be extended to Delta-Sigma Formats.