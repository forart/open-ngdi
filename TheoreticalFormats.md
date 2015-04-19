# Theoretical New Formats #

I want to discuss some of the new formats that have been mentioned before, but not yet implemented commercially or by amateurs (that I know of, please tell me if I'm wrong).

Specifically, the formats I am referring to are:
  * Multi-bit Delta Sigma, either 5 or 6 bit at 256fs (11.2892Mhz or 12.288Mhz) sample rates or higher, which would effectively be a "RAW" capture from today's best cutting edge ADC's.
  * 1-bit DSD at 256fs and higher sample rates. Anecdotal reports mention that 256fs appears to be the first point in 1-bit audio where the noise and signal don't interfere, therefore removing the need for noise shaping.

The reasoning behind the proposed format of 6-bit 256fs DSD, is the same reasoning that created DSD. The highest quality ADC's of today use a multiple order delta sigma converter, which is than processed into either 1-bit Delta sigma, or multi-bit PCM, losing data in either conversion. By capturing the "RAW" output of the ADC, all mathematical interpretation can be done at a later point, allowing conversion to other 'future' formats as they appear.

It should allow capturing the maximum obtainable quality in archiving priceless audio. All the disadvantages of DSD still hold true, lack of ability to perform manipulations or process without conversion, but now that we have moved past single bit delta sigma ADC's, the archival use of single bit DSD is questionable. I believe the "best" mathematical conversion is open to debate, and there is no perfect solution. By capturing the "RAW" output of a ADC allows the highest amount of care in selecting which algorithm is best in down conversion should allow the maximum quality to be obtained, and allows choosing a possibly superior conversion at a later date should another option arise.

I believe that this project has many applications beyond simply audio, perhaps an open-source SEM (scanning electron microscope) would benefit from a high speed interface for an ADC for capturing data for processing, Hams could use it for extending the utility of SDR (software defined radio's) to allow capturing/sending data, or a radio telescope project could benefit from more precise digitization, allowing linking up online and using aperture-synthesis to increase the effective aperture. Ultrasound systems and other medical imaging devices like MRI or CAT scans could be possibly utilize it, and lower starting costs for the developing world. GPR (ground penetrating radar) could be developed for the developing world to survey land quickly and cheaply, to find hidden dangers or resources.

The uses are endless, as we are in a society where there is a never ending need to capture, create, and analyze information. Open Hardware and Software is a revolution, and everything entered into the public domain can be reused and modified to find uses far beyond the original intention. For this reason I hope to create some momentum behind developing a General Purpose High speed ADC/DAC interface. Almost no design details exist as of now, except the proposed format. This is a similar project to the SDR-Widgit project, but with the expanded goal of supporting the "RAW" output of modern Delta-Sigma ADC's.

The need for a new archival and mastering format, as well as a format for scientific research in psycho acoustics, animal studies, ultrasonics, ultrasound, turbulence studies in a wind tunnel, and virtual reality is becoming more needed every day. As new technologies develop, in addition to computers becoming faster at an exponential rate, the need for easy ways to capture data accurately have never been greater.

I am hoping to start an open-source community that can help to develop a high quality high speed digital interface. This project will require an FPGA and custom programing and hardware to take the high speed multi-bit or single-bit data and accurately capture them. For audio purposes It will also be necessary to be able to output the data for playback through a DAC, without conversion to other formats.

- Alexander Countey, Sept. 17 2011

# Postscript #
The scope of this project is intentionally very broad, with the hope it will garner interest from as many developers as possible.