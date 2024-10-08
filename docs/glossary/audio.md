---
title: Audio Glossary
customDescription: Audio terms that you need to know
outline: [1,2]
---


<GradientCard title="音声用語集" tag="Audio Glossary" description="Audio concepts that you need to know." theme="turquoise"/>

<br>

<Authors page="audiog" />


![](/banner/bt.png)

<br>

# Basic Terms

### Audio File
| Terms | Details |
| ---- | ---- |
| Bitrate | The bitrate of an audio file is the number of bits of audio data stored per second, which can be variable or constant based on the encoding. |
| Lossy | Lossy compression, also known simply as lossy, is a data compression technique that reduces file size by selectively removing or approximating some of the original data from the source file. While this process discards certain information, modern algorithms are designed to do so in a way that minimizes perceptible differences from the original, making it nearly indistinguishable in quality for most users at certain bitrates. Common formats utilizing lossy compression include MP3, AAC, and OPUS. |
| Lossless | Lossless, also known as lossless compression, which is compression that preserves all data from the source file. Lossless compression is completely indistinguishable from the source file, while also reducing space and increasing efficiency of playback when compared to its uncompressed counterpart. Common lossless encoding formats include FLAC or ALAC. They are usually sourced from WAV files.  |
| Spectrogram | A measure of frequency density over time. A spectrogram can be viewed as a graph, with frequency density represented by color. The spectrogram can be used to scrutinize the quality of an encoding. |


### Release
| Terms | Details |
| ---- | ---- |
| Single | A music release containing 1 or 2 songs. |
| EP | Extended Play, a release usually containing 4 to 6 tracks.  |
| LP | Long Play, a full album release usually containing 10 to 12 tracks. |
| Album | An album is a collection of songs, either by a singular artist, vocalist, producer, or label. Sometimes, albums can even be compilations of multiple unrelated parties. They generally have a common theme, genre, or idea, known as a “Concept Album”, but they don't have to.  |
| Compilation | An album compiling tracks from different recordings of one or multiple aritsts. |
| Label | A company that publishes, distributes and promotes the music of their affiliated artists. The three biggest are [**Sony**](https://en.wikipedia.org/wiki/Sony_Music_Group), [**Universal**](https://en.wikipedia.org/wiki/Universal_Music_Group) & [**Warner**](https://en.wikipedia.org/wiki/Warner_Music_Group). |

### Hardware
| Terms | Details |
| ---- | ---- |
| IEM | Short for “In Ear Monitor”. These are much like earbuds, however, they have nozzles and tips attached to the end where audio comes out. This makes it such that the “monitor”, or speaker, goes “in ear”. Earbuds, alternatively, will rest on the ear without actually going in. The benefit of an IEM is that it creates a seal within your ear, which can allow for the bass response to be maintained much easier. More about IEMs can be found in the Some knowledge of audiophile equipment section.  |
| DAC | Short for “Digital-to-Analog Converter”. In terms of music, the DAC is the part of the chain that converts source files into analog signals that a headphone, speaker, or IEM can play back. More about DACs can be found in the Some knowledge of audiophile equipment section. |
| Amp | Short for “Amplifier”. In terms of music, the amp takes the converted signal from a DAC, or other analog source, and increases that signal's amplitude. This process is what makes audio louder. Any time you interact with a knob or volume rocker in order to make music louder or quieter, odds are you're interfacing with an amplifier. More about amps can be found in the Some knowledge of audiophile equipment section. |
| Speaker | Speakers shoot sound out towards the user. They consist of a subwoofer, woofer and tweeter. The subwoofer is usually disconnected from the woofer and tweeter pairing. |


![](/banner/af.png)

<br>

# Audio file

## Audio Signal

| Type | Description |
|-|-|
| Physical | Physical audio signals are produced by vibrating resonant objects. These vibrations travel through a medium (solid, liquid, or air) and form continuous wave functions. |
| Analog | An analog audio signal is a continuous wave function, characterized by a constantly changing voltage. Microphones or other receivers convert physical audio signals into analog signals. This continuous nature means the signal contains an infinite number of data points, making direct digital processing impractical. |
| Digital | A digital audio signal is also a wave function. It is discrete, meaning that there are only two logical states of potential. These waves can be interpreted as logical 1s and 0s, allowing for complex logical operations. |


::: details Pulse Code Modulation (PCM)
PCM (Pulse Code Modulation) is the most widely used audio encoding method. It involves sampling the audio signal at regular intervals and quantizing the amplitude of each sample into a discrete value. Music is generally recorded in a PCM format. Here are a few related terms for PCM:


- **Sample Rate**: The number of samples taken per second from the analog audio signal.
- **Bit Depth**: The number of levels used during quantization. These levels define the number of amplitudes available to the encoder. Higher levels mean a wider range of amplitudes per sample.
- **Channel**: The number of individual audio signals in the recording (e.g., mono, stereo).
:::

::: details Direct Stream Digital (DSD)


Direct Stream Digital (DSD), a product developed by [Sony & Philips](https://www.sony.net/Products/DSD/), is known for its high-resolution audio quality. However, DSD files are relatively rare due to their low popularity. Several factors contribute to this, including their large file size, the difficulty in mastering and editing during production, and the greater efficiency of PCM files in various aspects.


DSD is an audio encoding method that uses 1-bit delta-sigma modulation. It samples the audio signal at a very high samplerate, representing changes in signal density rather than amplitude levels, and has only 1 bit of amplitude. The most popular DSD standard is .dsf, but there are other standards as well.


![Analog Signal, PCM & DSD](https://www.sony.net/Products/DSD/images/img_1_en.png)


DSD files can be classified based on their sampling rate:


| DSD Type   | Sampling Rate           | Relation to CD Audio (44.1 kHz) |
|------------|---------------------|---------------------------------|
| DSD64          | 2.8224 MHz              | 64 times                           |
| DSD128         | 5.6448 MHz              | 128 times                          |
| DSD256         | 11.2896 MHz             | 256 times                          |
| DSD512         | 22.5792 MHz             | 512 times                          |
| DSD1024        | 45.1584 MHz             | 1024 times                         |


DSD’s high sampling rate allows for a wide dynamic range, even with a 1-bit depth. Factors like noise shaping and dithering also contribute to the audio quality. Noise shaping moves noise to the ultrasonic range. For example, DSD64 files start to see noise increase past 20kHz, requiring the DAC to filter it out. Higher DSD rates experience less noise rise, pushing it further into the ultrasonic range and making noise shaping more linear, which eases the DAC's job.


![Noise in DSD64 & DSD128](https://audiophilestyle.com/uploads/monthly_2014_12/dsd64-128.jpg.b549f3da738f0349755c8778cfbbb22e.jpg)

:::


## Analog to Digital

Analog audio signals are continuous sine waves. To process them digitally, we need to convert them into discrete signals. The discretization is performed on the amplitude and time domains.

- Discretization of time -> Sampling
- Discretization of amplitude -> Quantization


### Sampling
Sampling involves taking periodic cuts of analog signals, also known as PCM. More info can be found in [**sample rate**](#sample-rate).


![](/glossary/audio/sampling.jpg)

### Quantization
Quantization involves sampling an analog audio signal and converting it into a digital format. This process includes taking periodic samples of the audio wave and recording the amplitude of the analog signal per each sample. Because the recorded amplitude values are approximations of the original, there are inherent errors. These errors manifest as a noise floor within the sound wave. A higher bit depth reduces this error induced noise floor. This is because the quantization error is the difference between the original and quantized signals. Larger bit depths allow for more approximate quantizations, reducing the amplitude of the error signal.


![](https://upload.wikimedia.org/wikipedia/commons/b/b8/Quantization_error.png)


## Sample Rate
The amount of samples taken from the analog audio signal per cycle is known as the sample rate. As it's a per-second measurement, the unit is Hz (Hertz). Hertz are a measurement of frequency, or how many periods of a wave exist per second.

A higher sample rate means more data points are taken per second. This doesn't necessarily result in a higher quality signal. A higher sample allows for audio signals of higher frequencies, but for the communal frequency range, there are no advantages.

For listeners, 44.1KHz is sufficient to represent all humanly audible frequencies. 44.1KHz is the standard sampling rate for CDs, and 48KHz is the standard for DVDs and streaming services (originally brought forth to aid in timing with TV broadcasts). There is no functional difference between the two, beyond resampling issues that may arise between the mediums.

Higher sampling rates are often desirable by producers as it allows them modify the audio more flexibly without adding additional noise, but this is not relevant for playback. Higher sampling rates available on DACs are generally used for processing headroom (for e.g. low-pass filters), that may result in an audible difference.


::: details Dithering
Dithering is a process used when converting from different bit widths. Converting raw audio data to a different bit width will induce quantization errors during the conversion process. These are errors caused by averaging amplitudes. A dither signal can be applied to the audio before conversion, which is effectively noise. While noise may seem undesireable, it actually improves the quantization and signfigantly reduces the errors during the conversion. The noise is not percievable to humans, and does not effect the quality of a mix whatsoever.
:::

::: details Nyquist–Shannon Sampling Theorem
All audio signal sampling is based on this theorem. The theorem states that the sample rate has to be at least twice the maximum frequency of the analog signal to avoid aliasing. So, if the analog signal has a max frequency of 5kHz, the sample rate should be be at least 10kHz to reduce aliasing.


Another condition is bandlimiting. During the conversion of signals, high frequency distortion is added to the result. A band-pass filter helps to isolate the target frequencies from this distortion. Aliasing occurs if this distortion is not filtered. The folded wave interferes with the main wave and creates a new, unwanted sound wave.


![](/glossary/audio/nsst1.jpg)


To remove aliasing, a low pass filter (aka anti-aliasing filter) is added into both the ADC and DAC. Software will additionally include filters to remove aliasing in digitally generated audio signals. It's not practically possible to remove higher frequencies at the desired Nyquist frequency, so a buffer space is kept between the desired frequency and the Nyquist frequency. The buffer space depends on hardware capability.


![](/glossary/audio/nsst2.jpg)


>More details about the [Nyquist sampling theorem](https://en.wikipedia.org/wiki/Nyquist%E2%80%93Shannon_sampling_theorem).

:::


## Bit Depth


Bit depth indicates how many levels are used during quantization. Bit depth, also known as the number of levels, is defined by a power of **2<sup>levels of bit depth</sup>**.
- 8bit :mdi-arrow-right-thin: 256 levels
- 16bit :mdi-arrow-right-thin: 65,536 levels
- 24bit :mdi-arrow-right-thin: 16,777,216 levels


The increase in levels is exponential. The higher the level number, the closer the amplitude matching between analog and digital signals and the lower the amplitude of the resulting quantization noise. 


Increasing the bit depth blindly is counter-intuitive. For example, increasing the bit depth from 16 to 24 bits produces a barely perceivable enhancement. The file size, however, becomes much larger with the increase in depth.


::: details Dynamic Range
The dynamic range is the distance between the loudest and quietest sounds within a mix. The range can be calculated using this formula,

___

**Signal-to-Quantization-Noise Ratio = 20log(2<sup>bit depth</sup>)dB + 1.76dB**

___

This formula provides the following dynamic ranges: (without any dithering applied),
- 8bit :mdi-arrow-right-thin: 49.93dB
- 16bit :mdi-arrow-right-thin: 98.089dB
- 24bit :mdi-arrow-right-thin: 146.25dB


16-bit audio produces a maximum possible undithered dynamic range of ~96 dB, and with noise-shaped dithering applied, the dynamic range can increase upwards of 120dB. A average quiet home room won't have a significantly lower noise floor than 30 - 40dB. The minimum threshold at which a listener should experience a noise floor louder than that of ambient noise is well beyond the point where one would cause damage to their hearing. Bit depths greater than 16 are far more relevant for audio processing, rather than playback.


24-bit audio possesses a dynamic range exceeding the human hearing capabilities. With the increase in file size, it may be hard to justify the storage of these higher bit width files.

:::


## Bit rate
Bit rate is the amount of data streamed per second. For an audio file, there are three types:


| Bit Rate Types | Description |
|-|-|
| Constant (CBR) | The bit rate remains constant throughout the entire file (including bits storing silence). Since the bit rate is constant, the file size is more predictable. |
| Variable (VBR) | VBR adjusts the bit rate based on content complexity, which can lead to a more efficient use of bits, as well as smaller file sizes when compared to CBR encoding. |
| Average (ABR) | ABR is a middle ground between CBR and VBR. The bitrate is allowed to fluctuate, so long as an average value is maintained. This is considered an inferior standard when compared to the other two. |


## Codec
A codec is a standard used to encode and decode a data stream. Using codecs, data is stored in a container. Codecs are one of the most important factors in determining audio quality. There are several codecs used in the audio medium.


| Type | Codec |
|---|---|
| Uncompressed Lossless | WAV, AIFF |
| Compressed Lossless | FLAC, ALAC, APE, WavPack |
| Compressed Lossy | MP3, Vorbis, Opus, AAC |


### Uncompressed Lossless
Uncompressed lossless codecs are pretty old. They use CBR/Constant Bitrate encoding. CBR encoding ensures no data is lost, but the resulting file size is very large. WAVs consist of only a header, metadata, and raw quantization metrics. Devices can easily perceive this sort of encoding, leading to its relevance even today. As such, it's still widely used in music studios. As a consumer, they remain a bloated and unwanted format.


### Compressed Lossless
Lossless refers to lossless compression, which is compression that preserves all data from the source file. In terms of music, lossless compression is completely indistinguishable from the source file, while also reducing space and increasing efficiency of playback when compared to its uncompressed counterpart. Common lossless encoding formats include FLAC or ALAC. They are usually sourced from WAV files. They generally use VBR/Variable Bitrate encoding. The resulting file sizes are much smaller when compared to uncompressed lossless formats.

### Compressed Lossy
Lossy codecs aim to make file sizes small, even if it means compromising in quality. Quality of the sound varies wildly between formats and bitrates, with higher bitrates sounding better. Beyond the transparency level, everything will sound the same.

::: tip Transparency
Transparency means that the compression of the original file is accurate to a degree such that a listener can't distinguish between the compressed and original files. The level or threshold of transparency depends on listerns hearing ability, hardware, and the compression method. Since it's based on hearing ability, transparency is very subjective. The more efficient the codec is, the better it will sound **below its perceptually transparent bitrate**. In general, encoding quality follows the trend Opus > Vorbis ≈ AAC > MP3. The bit rates at which lossy audio files become transparent are subjective but the following are common choices of bitrates:


| Codec | Transparency Level |
|-------|---------------------|
| Opus  | 160-192 kbps            |
| Vorbis| 256 kbps                |
| AAC   | 256 kbps                |
| MP3 (CBR) | 320 kbps            |
| MP3 (VBR) | Between -V3 and -V0 |

:::

## Spectrogram

Spectrograms a.k.a spectral analysis are a reliable method to identify audio quality. Spectrograms plot the frequency spectrum across the time domain. Perceived loudness of these frequencies are represented by the color of the wave. The colors can then be decoded into a decibel rating from the legend on the right. This type of graph is useful in determining the sort of compression applied to an audio file. The depth at which these frequencies extend into the higher ranges indicate the type of compression utilized. Here, Spek has been used to analyze. The following are a couple of examples of different levels of quality:

:::tabs

== FLAC 24/48

![FLAC 24/48 (WEB)](/glossary/audio/spec/24.jpg)

The above figure is a spectrogram of a 24 bit, 48 kHz FLAC. A 48 kHz FLAC can support frequencies up to 24 kHz. This value comes from halving 48 kHz (following [Nyquist–Shannon Sampling Theorem](#sample-rate)).

== FLAC 16/44.1

![From Label (WEB)](/glossary/audio/spec/16.jpg)

This is a spectrogram of a 16 bit, 44.1 kHz FLAC file. A 44.1 kHz FLAC file can support frequencies up to 22.05 kHz. This spectrogram shows frequencies up to around 50dB extending up to 22.05 kHz, which is a great indicator of a truly lossless file.

![Trascoded from FLAC 24/48 (WEB)](/glossary/audio/spec/16t.jpg)

This 16 bit 44.1 kHz FLAC was transcoded from a 24 bit 48 kHz FLAC. Some of the data above 21.5 kHz is missing after the conversion. Although this conversion was from a lossless source and to a lossless source, it's technically not a lossless conversion. Data was lost, even though all of it is above the threshold of human hearing. This is due to the low pass filter applied below 20 kHz. A low pass filter has already been applied during the encoding of the 24 bit FLAC. Transcoding down to a lower sample rate applies this low pass filter again to prevent aliasing. This process usually causes the highest frequencies to be filtered out. This phenomenon can be observed when encoding in a different sample rate from the source. Either increasing or decreasing the sample rate causes some minor distortions between source files. Many different algorithms called SRC (Sample Rate Converters) exist and have varying degrees of effectiveness in mitigating these distortions. Generally, the distortions should not be perceivable by the average listener, but it's worth mentioning for sake of file integrity.

== MP3 320

![Transcoded 320kbps CBR from FLAC 16/44.1](/glossary/audio/spec/320.jpg)

This spectral is of a CBR 320kbps MP3 transcoded from a FLAC. The hard cutoff at 20.5 kHz is a good indicator of this sort of compression. Normally, frequencies wont extend all the way to 20.5 kHz. The frequency rolloff is much sharper than that of a FLAC file. A very loud noise must be present at higher frequencies in order for the data to persist to 20.5 kHz. Functionally, data will usually cutoff closer to 20.2 kHz. MP3s of any encoding style apply a softer cutoff, also known as a frequency shelf, around 16 kHz.

![](/glossary/audio/spec/sweep44.jpg)

The following is the proof that a CBR MP3 320 can reproduce frequencies at 20.5 kHz. 2 different sample rates were used, at 48 kHz and 44.1 kHz respectively. These spectrograms resulted from transcoding a 24 bit 96 kHz FLAC of a frequency sweep. The line is the frequency increasing linearly over time. The figure above depicts the source FLAC.

![](/glossary/audio/spec/sweep48.jpg)

2 lines are drawn on the figure. The top line is the highest perceivable frequency in the measurement, including the back distortion generated by the downsampling process. For the 48 kHz measurement, this line easily clears the 20.5 kHz mark. The second yellow line is measured from the highest perceivable frequency independent of the back distortion. This measurement appears to be at 20.5 kHz. Independent of how you choose to interpret the distortion, the MP3 contains the data.

![](/glossary/audio/spec/sweep3.jpg)

2 lines are drawn on the figure. The top line is the highest perceivable frequency in the measurement, including the back distortion generated by the downsampling process. For the 44.1 kHz measurement, this line appears slightly below the 20.5 kHz mark. The second yellow line is measured from the highest perceivable frequency independent of the back distortion. This measurement appears to be around 20.2 kHz. A 44.1 kHz MP3 probably can't hit 20.5 kHz.

== Opus 256

![Transcoded 256kbps VBR from FLAC 16/44.1](/glossary/audio/spec/256opus.jpg)

This spectral depicts a VBR Opus at 256kbps. The Opus codec is much more efficient than MP3, especially at lower bitrates. Opus 256 has a hard cutoff of 20 kHz, with no perceivable shelf, unlike MP3. Comparing the spectral to a FLAC, it almost looks like the frequencies about 20 kHz were chopped off and the rest of the spectrum was left untouched. This makes it a superior format in almost every way than an equivalent high bitrate MP3.

== MP3 V0

![Without 19.5 kHz cut-off filter](/glossary/audio/spec/v0.jpg)

This is a spectral of a V0 variable bitrate MP3, or V0 VBR MP3. V0 is the highest quality encoding preset. Frequencies extend up to about 22 kHz, much like that of a 16 bit lossless FLAC. This form of encoding is still a lossy compression, however. Much of the data beyond 19.5 kHz is heavily stripped out. The preserved data, for the most part, is also outside of the listenable range. Generally, this format is comparable to an MP3 CBR 320. CBR 320 is generally accepted as a better standard, in terms of raw data preservation. A 16 kHz shelf can be observed, a common result of MP3 encoding.

![With 19.5 kHz cut-off filter](/glossary/audio/spec/v0f.jpg)

This spectral is very similar to the previous, however, a 19.5 kHz low pass filter has been applied. This is a common practice among V0 encoding. As the data above 19.5 kHz has already been tampered with, and most of that data is transparent, some encoders filter it out by default. This process reduces file size, increasing the efficiency of the codec.

== MP3 192

![Transcoded 192kbps CBR from FLAC 16/44.1](/glossary/audio/spec/192.jpg)

This spectrogram is of a CBR 192kbps MP3. The source was a FLAC. Frequencies no longer extend past 19 kHz, and the MP3 shelf remains at 16 kHz.

== YouTube

![Opus 256 VBR (774)](/glossary/audio/spec/256opusyt.jpg)

YouTube commonly uses Opus for their music library. This spectral is of a 48 kHz 256 kbps VBR Opus file. The bitrate floats around 245 - 280 kbps at any given time. A hard cutoff exists at about 20 kHz, but frequencies occasionally persist beyond the cutoff. No discernible shelf is observable.

![Opus 128 VBR (251)](/glossary/audio/spec/128opusyt.jpg)

Audio quality can vary on youtube for a number of reasons, such as video playback quality and types of encoding. Audio on YouTube usually has an average of around 130 kbps. This spectral is of a 48 kHz 128 kbps VBR Opus file. The bitrate floats around 115 - 145 kbps at any given time. A hard cutoff exists at about 20 kHz, but frequencies occasionally persist beyond the cutoff. A slight shelf has been applied at 15.5 kHz. Compared to the 256 kbps Opus, aside from the slight shelf, the spectrals are very close. The quality loss, even at a much lower bitrates, is heavily reduced in the Opus standard.

== Spotify

![OGG Vorbis 320kbps (VBR)](/glossary/audio/spec/320ogg.jpg)

Spotify uses Vorbis encoding for its library. The above spectral is of a 320 kbps CBR Vorbis file. Comparing this to a FLAC encoding, frequencies beyond 19kHz suffer a soft shelving. Many of the frequencies still bypass the 19kHz threshold, but many quieter frequencies are filtered out at a quicker rate. The rest of the frequency spectrum is left untouched.

![OGG Vorbis 160kbps (VBR)](/glossary/audio/spec/160ogg.jpg)

This spectral is of a 160 kbps CBR Vorbis file. Comparing the 160 kbps Ogg to the 320 kbps Ogg, the lower bitrate suffers a decent amount of data loss throughout the spectrum. Frequencies as low as 2kHz seem to be missing between the two spectrals. Unlike a CBR MP3 at 160 kbps, frequencies are allowed to extend much higher. Instead of focusing on a frequency region to filter data out of, it instead targets areas within the music that the encoding process deems less necessary.

== Apple

![AAC 256kbps (VBR)](/glossary/audio/spec/256aac.jpg)

Apple uses their own AAC codec for lossy audio compression. The AAC version is up to 256kbps VBR . Bit rate for this file ranged from 216 - 313kbps. The frequency went upto 22kHz. The file has a cut-off near 22kHz which is persistent in lossless version too and was a file specific issue and not a codec issue. The spec is also free from the shelf issue like MP3 & OGG Vorbis.

The spec for the lossless 16/44.1:

![ALAC 16/44.1](/glossary/audio/spec/16alac.jpg)

== Case 1

![Kuuhaku no Sho by Taketeru Sunamori, Miyako Matsuoka](/glossary/audio/spec/instr.jpg)

Spectrals vary a lot depending on the genre of music. Ambient piano music could have less frequency data than genres such as mainstream pop. This spectral is of a lossless FLAC file. Frequencies still extend all the way to 22 kHz, but they are very low decibels in magnitude. A majority of frequencies don't even hit the 22 kHz point. Regardless, it's still a high quality, lossless encoding. Furthermore, lossless 44.1 kHz files don't actually have to hit as high as 22 kHz. If the producer decided to cut-off frequencies past a certain point, they wouldn't exist, lossless or not. This practice, however, is very rare. [This article](https://splice.com/blog/what-is-a-spectrogram/) is also a great explanation.

== Case 2

![One Last Kiss by Hikaru Utada](/glossary/audio/spec/2496eva.jpg)

These spectrals depict 24 bit 96 kHz FLAC encodes. A significant portion of the file is taken up by empty black space, devoid of audio information. This presents an argument such that a 24 bit 96 kHz provides nothing more than bloat. The files can easily be downsampled to a lower sample rate, while preserving a significant amount of the audio data. One last kiss, for example, would be a near lossless conversion. There are only a few moments where frequencies actually appear beyond about 25 kHz. A solid 23 kHz worth of data is essentially being allocated to nothing.

![Koi no Yukue by Akase Akari](/glossary/audio/spec/2496dress.jpg)

The My Dress-Up Darling ED makes much more use of the extra frequency headroom, however, it is already way beyond the threshold of human hearing. High sample rates for audio do play a role within production, allowing for a smoother experience if slowing down audio to a large degree. For playback, however, there is almost no reason for such a high sample rate audio file. If a song is released with such a high sample rate, there is an argument to be made for the preservation of that release. The average listener, however, will not perceive a difference in the form of downsampling the source, or even transcoding it to a lossy format.

:::

In short, analyzing a file can help determine the authenticity of the quality. A FLAC file cant always be taken at face value. If it sounds low quality, it could potentially be the result of a bad transcode. Software such as spek allows the user to analyze music and prevent the sharing of low quality, unwanted encodes.


## Container

Containers store all the data. The data is stored in different parts:
- **Header:** This section contains info about file format, size and signature.
- **Audio data:** This section is the main part. It contains the encoded audio file.
- **Metadata:** Metadata can contain info about title, artist, album, genre etc. 
- **Others:** There can be other parts too containing e.g. cue.

Audio files can also be embedded in non-audio specific containers, such as MKV and MP4, which include audio alongside video bitstreams.

## Audio Source


| Type | Source |
|---|---|
| Analog | Vinyl, tape |
| Digital | CD, DVD, Digital Store, Streaming |


- For **analog sources**, you have to use an [analog-to-digital converter](https://en.wikipedia.org/wiki/Analog-to-digital_converter) to get the digital file from the physical medium.
- For **digital sources**, audio files are already present in digital format. You have to use ripping software to rip from these.
- Among streaming services:
  - **Lossless**: Qobuz, Apple Music, Tidal, Amazon Music, Deezer
  - **Lossy**: Spotify, YouTube Music, SoundCloud

::: details More about analog sources

Two common analog sources are the vinyl and the cassette. 

- **Vinyls** are large discs that contain grooves in a spiral fashion. These grooves are proportional to that of the sin wave embedded into them. A needle can travel along these grooves in order to reproduce the signal as an alternating current. To achieve this, the vinyl is placed onto a device called a turntable, which spins the disc at a specific speed in order to accurately reproduce the sound. Due to the nature of the needle moving along the grooves, many claim that vinyls will lose sound quality over time. While this is very true, most people buying vinyls today will not listen to them often, so their lifespan can actually be quite long.   <br>
- **Cassettes**, also referred to as tapes, contain magnetic strips with sound information superimposed into them. This works by exposing the magnetic tape to an induced magnetic field. The field strength is proportional to the frequencies of the audio data being imposed. The magnetized particles then align in certain patterns within the tape, encoding the audio. Cassettes can be recorded and played back in a device known as a tape deck. Recording can be achieved on most tape decks, allowing the user to make tape recordings of whatever they like.
:::


## Transcoding

Transcoding means converting/encoding audio files from one codec/format to another. Audio can't be legitimately transcoded to higher quality since you can't generate new details after compression has been applied. That's why you shouldn't transcode
 -  lossy into another lossy because you will lose more details during transcoding.
 -  lossy into lossless since it will be just a waste of space & no audio quality improvement.

::: tip The process
To learn how to transcode using Foobar2000, [read this guide](/guides/music/transcoding.md).
:::

## Other File types

### .log
Log files are generated during the ripping process. It contains necessary information to show the integrity of the hardware, errors, as well as the ripping process etc. Users should never modify a log file. [**Example**](https://rentry.org/wlogx) of a log file.

### .cue
Cues contains metadata about the tracks, including their start and end points, titles, and performers. It can also include additional details such as gaps between tracks and pre-gap data. Cue files are used by media players and burning software to accurately recreate the original CD's structure. This ensures the correct track order and gaps are maintained, enabling a faithful reproduction of the CD's layout when played back or burned to a new disc. cue files are used to make one singular audio file act like it has tracks, as opposed to applying to a list of files. [**Example**](https://rentry.org/wotacue) of a cue file.

### .m3u8
m3u8 files are used for playlists of audio. It contains a list of paths to your local audio files (like songs or podcasts) in order. The difference between a m3u and a m3u8 is that m3u uses ASCII (which only supports English characters) and m3u8 uses UTF-8 (which supports characters of other languages too).

```plaintext
#EXTM3U

# Song Title 1
# Duration: 123 seconds
#EXTINF:123,Song Title 1
C:\Music\song1.mp3

# Song Title 2
# Duration: 200 seconds
#EXTINF:200,Canción 2
C:\Music\canción2.mp3

# Song Title 3
# Duration: 180 seconds
#EXTINF:180,歌曲 3
C:\Music\歌曲3.mp3
```

![](/banner/hw.png)

<br>


# Hardware

<br>

Hardware refers to the devices within the signal chain to reproduce listenable audio. The 3 core devices are the Dac, Amp, and playback device. To briefly explain the signal chain, digital audio needs to be sent to a DAC in order to be converted into a usable analog signal. That analog signal is then amplified to bring it to a listenable volume. Finally, a headphone, IEM, or speaker is plugged into the amplifier to reproduce the sound. This chain holds true for any form of digital media, but analog sources do not require a DAC, as the audio signal is already in the analog form.

![](/glossary/audio/mermaid.png)

## DAC

The DAC, or Digital to Analog Converter, takes in digital bitstreams and converts them into analog signals. They come in two distinct form factors: desktop devices or dongles.

1. **Dongles:** A dongle is intended for use with a phone, and generally has an amplifier built in. This makes the dongle a completely standalone device, and you only need to plug it in to make it work. 
2. **Desktop DAC:** The desktop DAC, alternatively, will rest on a surface. It's much larger and isn't intended to be used portably. It takes in external power from the wall and can offer unbalanced or balanced analog outputs. Desktop DACs are intended to be paired with an external tabletop amplifier. Combination desktop DAC and Amp units exist, although they are less common.

![](/glossary/audio/dac.png)

## Amp

The amp, or amplifier, takes in analog signals and outputs an amplified version. This process makes the signal louder. An amp can take in a signal from either a DAC, or some other analog source.

There are two types of amplifiers: unbalanced, and balanced.

- **Unbalanced amplifiers** take in an unbalanced signal, such as one fed from an RCA cable, and outputs an unbalanced signal. An unbalanced signal consists of 3 channels: a left audio channel, a right audio channel, and a ground wire.
- **Balanced amplifier** takes in a balanced signal, such as one fed from an XLR cable, and outputs a balanced signal. A balanced signal, unlike its unbalanced counterpart, has 2 copies of each of the left and right channels. Functionally, balanced signals are utilized to decrease the amount of noise a wire picks up as a signal travels along it. Practically, this noise shouldn't exist in shorter unbalanced connections, such as those that would be used on a headphone or speaker. However, balanced signals operate on a higher voltage, which allows your amp to output a higher wattage overall.

The primary difference in amplifiers is how much wattage they can output. Amplifiers come in the form of dongles, desktop sized devices, or large AVRs intended for speakers. Dongles will (generally) output less wattage than desktop sized amplifiers, and desktop sized amplifiers will provide less wattage than an AVR. Dongles can have a DAC embedded within them, making them convenient portable all-in-one solutions. You can tell by the type of connector they use as an input. If the dongle terminates in a connector such as a usb-c, which is a digital input, it’s going to have a DAC. 

![](/glossary/audio/amp.png)

## Playback Device

Playback devices come in many forms, but only the most common will be covered. Specifically the headphone, IEM, and speaker.

###	Headphone


A headphone is 2 speaker drivers held together by a headband. They can be wired, bluetooth, or wireless with a dongle. To briefly explain the differences: 

- Wired headphones are passive devices that can be plugged into anything with an audio jack. If it terminates in a 3.5mm or usb-c, then it may be plugged into its respective port. Bluetooth headphones are wireless, although many still offer a cable for an optional passive use.

- Audio sent via bluetooth is always compressed with lossy compression, and even with modern bluetooth standards, there is no getting around that. Wireless headphones aren't restricted by the bluetooth encoding standards. The audio may be sent losslessly to the device. The downside is that they typically require a hub or wireless dongle to connect to. This severely limits the amount of devices they could potentially be connected to.

Headphones can have two distinct varieties. Closed back & Open back headphones.

- **Closed back** designs involve a sealed backplate to enclose the driver. This is the most common design, although it presents a larger challenge for acoustically tuning the headphone. When a driver is sealed, the audio that is hitting the backplate must be properly filtered in order to provide a pleasant sound for the listener. This filtering can be achieved with physical design solutions, such as foams, felts, or vents for certain frequencies.

- **Open back** headphones, alternatively, utilize a perforated backplate. This backplate allows sound to be shot outside of the headphone, yielding a less restrictive physical design. There are other benefits, such as open backs generally producing a wider soundstage, which is how far away a sound is perceived from the listener. Open backs are regarded as being easier to tune than closed backs, and some believe the sound of an open back is “more natural.” Even with these benefits, open backs remain a less commonly owned variant. Open back headphones project sound outside of the headphone. Most users seek privacy in the content they listen to, making a closed back a more private and desirable option.

### In Ear Monitor

In ear monitors, or IEMs for short, are devices intended to be inserted into the ear for audio playback. This allows them to be a more private option for listening to music while retaining an even frequency response. IEMs are built similarly to earbuds, however, they are designed with nozzles that the music is shot out of. These nozzles are fitted with eartips, which are then inserted into the ear and suspended by the tip. This allows the tip to seal within the ear, decreasing the sound that leaks out while increasing the depth at which sound can travel. This process especially enhances the bass response.

::: details More
IEM configurations can be very complex. They commonly utilize multiple different drivers in a single shell. These multi driver type configurations are referred to as “hybrids”, and are very common within the IEM space. The main argument for their existence is that no one driver can perfectly reproduce the audio spectrum. Some driver types fail at applications that other driver types may excel at. Configuring an IEM with different types of drivers, and designing a crossover to split frequencies between these drivers should enhance the overall fidelity. In practice, there are very good single driver, multi driver, and hybrid driver configurations on the market. It all comes down to user preference. 
:::

### Speaker

Speakers are drivers within enclosures a set distance away from the listener. The sound travels, bounces, and fills up the room until it reaches the listener, creating the effect of a vast wall of sound. Configurations vary more widely than their headphone and IEM counterparts, but their fundamental concepts of sound reproduction are the same. The primary advantage of speakers is their lack of size restrictions, allowing for larger and more complex designs to exist.

A singular driver will not do a good job at reproducing the entire sound spectrum. Generally, a driver will have a portion of sound it excels at. This is especially true for drivers used in speakers. Speakers consist of 3 driver types: 
1. Subwoofer
2. Woofer and
3. Tweeter.

Each driver type handles a different part of the frequency spectrum. Most commonly, a woofer and tweeter will be paired within the same enclosure. A subwoofer would be detached and contained within its own enclosure. 

| Driver | Work |
|-|-|
| Subwoofer | The subwoofer, which is also the name for the type of speaker, is the driver that specializes in very low frequencies. These are at and below 80Hz, but many subwoofers allow the user to increase or decrease this ceiling. |
| Woofer | The woofer is optimized for the middle frequencies. The middle frequencies are defined by the crossover between the subwoofer and the woofer, but from around 80 Hz to 2 kHz is common. The crossover should be defined by the capabilities of the woofer, such that the subwoofer can make up for where the woofer lacks. |
| Tweeter | The tweeter will handle frequencies between around 2kHz-20kHz. Tweeters can play frequencies beyond 20kHz, but humans aren’t able to perceive them. A woofer paired with a tweeter is the most common speaker configuration, known as a 2-way speaker. |

Speakers achieve frequency separation between drivers with use of a crossover. This crossover can be passive or active, and functions as a filter for the frequencies. These frequency separations are not instantaneous, as frequencies will bleed into both drivers at the crossover point. This is both due to a limitation of frequency filtering circuits as well as making the crossover sound more natural.

::: details More

Speakers come in two distinct types, active or passive units.

- **Passive units** are unpowered. These devices only have speaker terminals in the back, intended to be hooked up to an external amplifier or AVR. Sound is played back as amplified signal passes through them. An external DAC and amp are required to make use of them (unless the source was analog, in which case, only an amp).
- **Active units**, on the other hand, are powered. This implies they contain amplification circuitry (and potentially DAC circuitry) internally. Usually, these powered units will take a DC barrel plug, or a standard IEC cable in the back. They also can provide analog inputs for the internal amplifier, such as RCA or XLR. Digital inputs may also be present if the speaker contains a DAC, such as toslink optical or Bluetooth. These components, as well as the circuitry, are mounted onto a plate and screwed into the speaker. Subwoofers are commonly active units, as they allow for much more control over the subwoofer’s crossover.

:::

## Frequency Response

::: info Summary
The frequency response shows how something sounds across the frequency spectrum, in terms of gain. It can be used to quickly understand how loud the bass, mids, and highs are reproduced. 
:::

No one driver will reproduce the entire listenable frequency spectrum, that being 20 Hz to 20 kHz, flatly. The loudness of frequencies will always vary throughout the spectrum. The measure of the magnitude of response of the frequency spectrum is known as the frequency response. The frequency response would be the most perceivable difference between playback devices.  <br>

The following image is the frequency response of a common headphone, the Sennheiser HD 600:

![](/glossary/audio/crinacle.jpg)

The blue and red lines are the left and right drivers of the headphone. The X axis is the frequency spectrum, increasing from 20Hz to 20kHz, and the Y axis is the perceived loudness. Just for example, at around 30Hz the graph shows a gain of about 60dB. The black line is what the raw measurement was compensated to. That means that the original slope of the blue and red lines were superimposed on the curve depicted by the black line. This is done because the human ear processes frequencies in a strange, non linear manner. The compensation is an attempt to try to more accurately depict how the headphone would sound to the human ear.   <br>

The response can be analyzed like so: Crinacle adds the bold lines at 100Hz and 1kHz to separate the bass frequencies from the mid frequencies, and the mid frequencies from the high frequencies. The bass section contains bass tones, such as a kick drum. The mids contain a majority of the sounds in a song, everything from vocals to guitars to synths. The highs mostly consist of a niche subset of instruments, such as cymbals and brass instruments, as well as detail for the lower frequencies. Female vocals may also bleed into this range. The most noticeable portion of a response like this is how the bass is rolled off under about 80Hz, meaning it gradually decreases in gain down to 20Hz. The overall response tries to stay flat, or neutral, but the high frequencies suffer some dips and peaks throughout the spectrum.


## Equalization

::: info Summary
Eq allows for altering of playback. Sound can be flavored to a user’s preferences, with no cost to the user. 
:::

Equalization, also shortened to eq, allows you to alter the frequency response of a playback device. This can be very useful if a particular section of the frequency response is not so pleasant to listen to, such as it being too loud or too quiet. Equalization can easily be performed on a desktop computer or a mobile phone, although there are also dedicated devices. 

While this is a very powerful tool, there are still limitations to equalization.  If the users wanted to make certain frequencies louder, it's not as simple as raising the level. For example, the user wanted 80 Hz tones to appear louder. In an eq, those tones are raised by \+3 db. This would make 80 Hz frequencies louder, however, the eq is digitally amplifying the signal. Digital audio has a maximum loudness it can achieve, and if that loudness gets exceeded, the sound will distort. There is a simple solution to this problem. Most equalizers have a feature that sets the maximum gain across all bands to 0db. This is basically shifting the entire equalization down until the top most slider is equal to 0db. In other words, instead of making a sound louder, you're making the rest of the frequency spectrum quieter. In order to make up for this loss in gain, more analog amplification is required to meet the difference.

The second limitation of EQ is that it can't make a bad piece of hardware good. Eq can definitely make any piece of hardware sound better, but it can't turn a $10 gas station headphone into something that would please an audiophile. If a piece of hardware isn't offering a fidelity the user desires, the user should look at better hardware to satisfy their desires.   

![](/glossary/audio/eq.png)

This is an example of the bass boost eq profile in musicbee. The preamp is set to \-6dB, which is larger in magnitude than the largest magnitude of the boosted frequencies. This ensures that no peaking occurs on the output. Frequencies below 1 kHz are gradually increased, emphasizing these frequencies in playback. Frequencies around 32 Hz receive the greatest effect.


![](/banner/mg.png)

<br>

# Japanese Music Genres

<br>

There are multiple genres that are distinctly Japanese, all with different origins and established in different periods of time. The following are modern genres that still hold relevance within a majority of listeners today:


## Vocaloid

::: tip Vocaloid & Vocaloid
The genre vocaloid is name after the voice synth [Vocaloid](https://www.vocaloid.com/en/) (by Yamaha). But as a genre, it counts every song produced by voice synth. For example:  [Synthesizer V](https://dreamtonics.com/synthesizerv/), [CeVIO](https://cevio.jp/), [OpenUTAO](https://www.openutau.com/) etc.
:::

Vocaloid remains an icon of the early to mid 2000s. With the help of [NicoNico Douga](https://www.nicovideo.jp/), a japanese video sharing platform, Vocaloid would skyrocket in popularity within the underground doujin scene. [Hatsune Miku](https://en.wikipedia.org/wiki/Hatsune_Miku)’s cover of "[**Ievan Polkka**](https://youtu.be/widZEAJc0QM)" in particular would garner the genre massive exposure. (A remastered version of the track can be heard [here](https://youtu.be/z5Ub37hEQFo?si=EuYtiGZkcZrrYooX).)

Vocaloid is much broader than just Hatsune Miku. With its extensive array of voice banks, Vocaloid encompasses a huge variety of genres and styles within its own umbrella of synthetically constructed vocals. While not a concrete number, there are easily around 100 officially licensed Vocaloid voice banks as of 2024, not counting rereleases. Factoring in vocal synths, as well as the publicly available utau voice banks, this number becomes astronomically higher. Essentially, the capabilities of Vocaloid software allow for an endless amount of user expression.

Vocaloid would slowly gain traction after the release of Vocaloid 2. The doujin scene in particular would latch onto the easy to use software to make up for the lack of a vocalist. The voicebanks were there to use, and could be warped to whatever sound and aesthetic the producer desired. Hatsune Miku in particular would become a sort of icon for the genre, with her design being plastered all across the internet and Japan alike. Sega would consistently tie Hatsune Miku into spinoff games, such as the Project Diva rhythm game series. The internet would create animations in software such as Adobe Flash, as well as fanart of Hatsune Miku. The art and animations would accompany releases in a sort of Vocaloid mixed media production. All of this tied into mass exposure for the genre, and especially the brand. Even today, these traditions are still being honored in modern Vocaloid releases.

Everything from jpop to metal to hard trance is fair game for Vocaloid. While the term refers to a genre in of itself, it's more akin to how non-specific something like “female vocals” would be. The only qualification for a Vocaloid song is for it to contain vocals from some sort of vocaloid/utau voicebank. Its low barrier to entry has found a niche in pretty much every modern genre.

Some popular vocaloid producers consist of [**Kikuo**](https://www.youtube.com/@kikuo_sound), [**PinocchioP**](https://www.youtube.com/@pinocchiop), [**Wowaka**](https://www.youtube.com/playlist?list=PLnYDKMNVcwf5ihkhxeAhyFPkbs9--Xukc) and [**Mitchie M**](https://www.youtube.com/@MitchieM). 

## Shibuya-kei

[Shibuya-kei](https://en.wikipedia.org/wiki/Shibuya-kei) was born in the 90s and died in the early 2000s. The Shibuya part of the name points to the origin of sales of the music and kei points to a (supposed) type of person of the [Shibuya district](https://maps.app.goo.gl/NSagswXtigf5eV2b7). The sound is most concretely pop, but it pulls its inspiration mostly from various different types of jazz.

Bossa nova in particular seems to be a large inspiration. The genre featured a lot of french vocalists, and their musical influences bled into the genre. This can be seen within Shibuya-kei’s most recognizable group, Pizzicato Five, as well as vocalists such as Kahimi Karie. Cornelius more or less spearheaded the genre, with many self compositions as well as compositions released under their own label “Trattoria” dominating the scene. While the genre was quick to start and quick to die, it left an impact. Foreign listeners in particular were fond of the genre and it still remains an influential genre within Japan.

Honorable mention Cibo Matto’s [**Stero Type A**](https://www.youtube.com/playlist?list=OLAK5uy_nBKsSYZljXguvcs8cKCp2YwU3a2-tVF5U).

## Denpa
Denpa music is defined vaguely, but it consists of music the average person would deem “weird”. Not in the avant garde experimental kind of way but usually in the more otaku influenced… synth rainbow vomit kind of way. Denpa music doesn’t really pay its origin to any one subculture in particular, however, it is commonly associated with the otaku. Its otaku association, and eventually catering of the genre to, helped to proliferate and solidify its infamy.

The actual origin of the genre lay in songs that were considered creepy. Repeated nonsensical vocals over cutesy soundfonts made for an uncomfortable listening session. This would further develop with the rise of the term “denpa” as a way to describe delusional and mentally unwell individuals (more can be read about its origins [here](https://en.wikipedia.org/wiki/Denpa\_song)). The genre of music would evolve into songs that contained menhera themes, otaku themes, or themes most of Japanese society at the time would not be comfortable listening to. A lot of parallels would be drawn to genres such as jpop and jcore, however, most people who make denpa music tend not to associate with other genres in order to keep its underground origins intact.

Popular artists/producers/groups/circles in the scene consist of [**Nanahira**](https://www.youtube.com/@Nanahira_Confetto) and [**iOSYS**](https://www.youtube.com/@iosys_official).


## Jpop

Jpop, Japanese pop, is pop music with origins in Japan. The sound is distinct from western pop, in that a lot of influences from Shibuya-kei (see above) and modern mexican pop can be observed within the scene. The genre gets marketed internationally much like that of Kpop, but to a less impactful degree. Due to a high otaku presence within the genre, there arise opportunities for more risky, experimental productions to be funded. With the large ethnographic appeal to the Jpop scene, a unique situation arises where vastly different styles of Jpop are allowed to rise to the top. The genre can be perceived as being more diverse than a western counterpart, and it probably is to a degree.

Popular Jpop artists to check out could be [**REOL**](https://www.youtube.com/@reolch), [**Ado**](https://www.youtube.com/@Ado1024), or [**Haru Nemuri**](https://www.youtube.com/@harunemuri).

## Doujin (music)
Doujin, specifically Doujin music, is the otaku indie scene of music within Japan. While not all of it is explicitly otaku, a large majority of it is associated with the culture. This is music being released on CD-Rs at events such as Comiket, Reitaisai, or M3. The music can also be released digitally should the circle/individual want it. There's no explicit genre, but the releases are usually from small and tightly knit groups called circles (if not individuals).

A couple doujin artist/circles worth checking out consist of [**Shibayan Records**](https://www.youtube.com/@ShibayanRecords), [**Release Hallucination**](https://www.youtube.com/@ReleaseHallucination), or [**Akatsuki Records**](https://www.youtube.com/@Akatsuki-Records).

## Jcore
Jcore specifically refers to the Japanese core style music scene, although the Japanese electronic scene as a whole is incredibly influential. Many international electronic music fans are aware of and actively listening to the Japanese electronic music scene at large. A big reason for this is the exporting of rhythm games from japan. A majority of doujin music exists within the Jcore sphere, and many doujin music circles sell rights to their music to rhythm game companies. As such, the Jcore scene sees mass international exposure to people within the rhythm game subculture.

Producers in the J-Core scene worth checking out consist of [**DJ Sharpnel**](https://music.youtube.com/channel/UCkuWrVX6ME6koqF5AehTkmw) and [**TORIENA**](https://www.youtube.com/@torienaofficial).

## Idol

Idol music falls under the multi-media umbrella of Japanese idol culture. Idols are teenage girls that are over-marketed into superstars for an otaku audience. Ideas of escapism, maximalism, and aesthetics are core to the subculture. Idols normally don't have prior knowledge from a performance background. Rather, studios will engineer idols into performance artists with strict and unorganized schedules. Many social freedoms are restricted, such as visiting family and drinking/smoking. A distinct image must be upheld, an image that has been core to the subculture since the beginning. 

The music itself consists of a variety of genres. Denpa, Jpop, and Jrock are all fair game for idol groups. Experimentation is welcome within the genre, but the music is going to be dictated by the studio that hired the idol. Groups such as Babymetal are iconic for combining metal with more popish, traditional idol vocals. 

::: info Where to purchase Japanese Music?

Give the [Wotaku music page](https://wotaku.moe/music\#purchase) a look. Both [**Ototoy**](https://ototoy.jp/top/) and [**Bandcamp**](https://bandcamp.com/) house a lot of high quality japanese music, both from the mainstream as well as the underground. Each storefront allows the user to save music purchases to an account. As long as the service is live, music can be redownloaded indefinitely. Both services also offer lossless, as well as 24 bit lossless.

For physicals, [**Suruga-ya**](https://www.suruga-ya.com/en/index) is a Japanese second hand market with a good english translation and international shipping feature. Otherwise, a website such as booth-pm or melonbooks can be navigated with minimal trouble, however, a proxy shipping service must be utilized. 
:::
