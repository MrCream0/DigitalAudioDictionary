# Digital Audio Programming Basics

## Table of Contents

1. Introduction to Digital Audio
2. Sampling and Quantization
3. Audio File Formats
4. Audio Playback
5. Digital Signal Processing (DSP) Basics
6. Real-Time Audio Processing
7. MIDI and Audio Synthesis

---
## 1. Introduction to Digital Audio

Digital audio is a representation of sound using binary data. It involves converting continuous analog audio signals into discrete digital samples for processing and storage. Key concepts to understand:

- **Analog vs. Digital**: Analog audio signals are continuous waveforms, while digital audio consists of discrete samples.
    
- **Sampling Rate**: The number of samples taken per second. Common rates are 44.1 kHz, 48 kHz, and 96 kHz.
    
- **Bit Depth**: The number of bits used to represent each sample. Common depths are 16-bit and 24-bit.
    

---
## 2. Sampling and Quantization

- **Sampling**: The process of measuring an analog audio signal at regular intervals to create digital samples.
    
- **Nyquist Theorem**: States that to accurately represent a signal, the sampling rate must be at least twice the highest frequency present in the signal.
    
- **Quantization**: The process of converting continuous amplitude values into discrete levels using a fixed number of bits.
    

---
## 3. Audio File Formats

- **WAV**: Uncompressed audio format. Simple structure, widely supported, but large file sizes.
    
- **MP3**: Lossy compression format. Smaller file sizes, but some audio quality loss.
    
- **FLAC**: Lossless compression format. Smaller than WAV, retains original audio quality.
    
- **AIFF**: Similar to WAV, commonly used on Apple platforms.
    

---
## 4. Audio Playback

- **Audio APIs**: Application Programming Interfaces for audio playback include:
    
    - Core Audio (macOS, iOS)
    - DirectSound (Windows)
    - ALSA/PulseAudio (Linux)
- **Buffering**: Storing audio samples in a buffer before playback for smooth output.
    
- **Sample Rate Conversion**: Changing the sampling rate to match the output device.
    

---
## 5. Digital Signal Processing (DSP) Basics

- **Filtering**: Removing or emphasizing specific frequency components of an audio signal.
    
- **Time-Domain vs. Frequency-Domain**: Representing audio in the time domain (waveform) or frequency domain (spectrum).
    
- **Fast Fourier Transform (FFT)**: Algorithm to convert time-domain data into frequency-domain data.
    

---
## 6. Real-Time Audio Processing

- **Low-Latency Audio**: Minimizing delay between audio input and output for real-time applications.
    
- **Circular Buffer**: A data structure for efficient audio streaming and processing.
    
- **Audio Effects**: Implementing effects like reverb, delay, and distortion in real-time.
    

---
## 7. MIDI and Audio Synthesis

- **MIDI**: Musical Instrument Digital Interface; used to communicate musical events like notes, pitch, and velocity.
    
- **Synthesis Techniques**:
    
    - **Additive Synthesis**: Creating complex sounds by combining multiple sine waves.
    - **Subtractive Synthesis**: Filtering harmonically rich waveforms like sawtooth or square waves.
    - **Granular Synthesis**: Manipulating tiny audio grains to create textures.
