# DSP Filter Design Exercise

This repository contains a Jupyter Notebook exercise on designing high-pass filters for Digital Signal Processing (DSP).

## Overview

The goal of this exercise is to simulate a voice signal containing a range of frequencies mixed with an unwanted DC offset, and to design and compare different digital filters to effectively remove the DC component while preserving the voice frequencies.

The notebook guides you through the following steps:
1. **Signal Generation**: Simulating a voice signal mixed with a DC offset.
2. **Simple High-Pass Filter (Baseline)**: Analyzing the performance of a basic first-difference filter ($y[n] = x[n] - x[n-1]$) and observing its slow roll-off.
3. **FIR Filter Design (Windowed Sinc Method)**: Designing a Finite Impulse Response (FIR) filter using `scipy.signal.firwin`. You will experiment with the number of taps and cutoff frequencies to observe the effects on roll-off sharpness and signal quality.
4. **IIR Filter Design (Butterworth)**: Designing an Infinite Impulse Response (IIR) filter using a Butterworth design to achieve a sharper roll-off with fewer coefficients, and understanding the trade-off of non-linear phase.
5. **Frequency Response Comparison**: Comparing the frequency responses (magnitude) of all three filters.
6. **Output Spectra Comparison**: Visualizing and comparing the frequency spectra of the filtered signals.
7. **Time Domain Comparison**: Examining the filtered signals in the time domain to see how well the DC offset is removed.
8. **Audio Playback**: Listening to the resulting signals (if supported in your Jupyter environment) to hear the qualitative differences between the simple HPF and the FIR/IIR HPF outputs.
9. **Quantitative Comparison**: Measuring frequency preservation and DC suppression numerically.
10. **Phase Response Comparison**: Understanding the difference between linear phase in symmetric FIR filters and non-linear phase in IIR filters.

## Requirements

To run this notebook, you will need a Python environment with the following packages installed:
*   `numpy`
*   `scipy`
*   `matplotlib`
*   `ipython` (for audio playback)
*   `jupyter` (to run the notebook)


