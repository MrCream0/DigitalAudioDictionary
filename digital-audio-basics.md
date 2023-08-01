
## Digital Audio Basics

## 1. Analog To Digital Conversion (ADC)

+ The process of converting continuous analog audio signals into discrete values for storage and processing.

---

## 2. Sample rate

+ the number of samples taken per second to represent an analog audio signal digitally (44.1 is 44100 samples per second or how many times the samples of the recording are taken).
+ Measured in Hertz (Hz).
+ Common sample rates include 44.1kHz(CD quality), 48 kHz(DVD quality), and 96kHz(high-resolution audio).

--- 

## 3. Sampling

+ The act of measures the amplitude of the analog audio signal at regular intervals (samples) to create a digital representation.

--- 

## 4. Nyquist Theorem

+ States that the sample rate but be at least twice the highest frequency present in the analog signal to avoid aliasing.
+ The highest frequency that can be accurately represented is referred to as the Nyquist frequency.
 If the sample rate is 44100 the Nyquist frequency would be half of that 22050hz.
 
---

## 5. Bit Depth

+ Determines the number of bits used to represent the amplitude of each other audio sample.
+ Higher bit depths result in more precise representation and higher audio fidelity.
+ Common bit depths include 16-bit(CD quality), and 24-bit(high-resolution audio).

--- 

# 6. Quantization

+ The process of approximating the continuous amplitude values of an analog signal by assigning discrete numerical values to each sample.
+ Quantization error occurs due to the finite number of available discrete values, leading to a loss of audio quality.

---

## 7. Dynamic Range

+ The difference between the softest and loudest sounds that can be accurately captured and reproduced in digital audio.
+ Expressed in decibels(dB).
+ Determined by the bit depth: higher bit depths allow for a wider dynamic range.

--- 
## 8. Audio File Formats

+ Containers used to store digital audio data
+ Common formats include WAV(uncompressed), MP3(lossy compression), FLAC(lossless compression), and AAC(advanced audio coding).

---

## 9. Dithering

+ A technique used to reduce quantization of digital audio signals using mathematical algorithms.
+ Adds low-level random noise to the audio signal to smooth out the transition between quantization levels.
See [[https://digitalsoundandmusic.com/5-3-7-the-mathematics-of-dithering-and-noise-shaping/]]
for a more depth to dithering

---

## 10. Digital Signal Processing (DSP)

+ Manipulation and processing of digital audio signals using algorithms.
+ Used for various audio effects, equalization, filtering, and more.
More Here [[https://www.sciencedirect.com/topics/computer-science/digital-signal-processing-algorithm#:~:text=Digital%20signal%20processing%20algorithms%20are,known%20as%20operations%20or%20ops.]].

---

## 11. Aliasing

+ Aliasing occurs when high-frequency components in the analog audio signal are not adequately represented due to insufficient sample rate. This results in unwanted artifacts in the digital audio signal.

--- 

## 12. Anti-Aliasing Filter

+ An analog or digital filter used to remove frequencies above the Nyquist frequency before sampling, preventing aliasing.

---

## 13. Digital-To-Analog Conversion(DAC)

+ The process of converting digital audio data back to the continuous analog signals for playback through speakers or headphones.

---

## 14. Bit Rate

+ The rate at which digital audio data is transmitted or processed, measured in bits per second(bps).

---

## 15. Lossy Compression

+ Audio compression method that permanently removes some audio data to reduce file size, leading to a loss of audio quality.
+ Commonly used in formats like MP3 to achieve smaller file sizes.

---

## 16. Lossless Compression

+ Audio compression method that reduces file size without sacrificing audio quality by removing redundant data.
+ Formats like FLAC and ALAC use lossless compression

---

## 17. Pulse Code Modulation(PCM)

+ The most common method of digital audio representation.
+ PCM represents audio samples using binary code, where each sample is quantized and represented as a binary number.

---

## 18. MIDI (Musical Instrument Digital Interface)

+ A protocol used to communicate musical information between digital devices, primarily  used for controlling synthesizers and other musical equipment.

---

## 19. Audio Interfaces

+ Hardware devices used to connect audio sources and outputs to a computer for recoding and playback.

---

## 20. Latency

+ The delay between an audio signal entering a system and its output, which can impact real-time audio processing and monitoring.

---

# 21. Equalization(EQ)

+ The process of adjusting the balance of frequencies in an audio signal using equalizers.
+ Used for tonal shaping and correcting frequency imbalances.