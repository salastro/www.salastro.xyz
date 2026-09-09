---
id: "signal-processing"
title: "Signal Processing"
group: "focus"
level: 1
val: 10
date: "2024-03-15"
img: "https://images.unsplash.com/photo-1760978632061-ad00f48789ae?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3w3Nzg4Nzd8MHwxfHNlYXJjaHwxfHxkaWdpdGFsJTIwc2lnbmFsJTIwd2F2ZSUyMGRhcmt8ZW58MXx8fHwxNzcwODIyOTY1fDA&ixlib=rb-4.1.0&q=80&w=1080"
tags: ["DSP", "Stochastic", "Estimation"]
projects: ["proj-dsp-fpga"]
concepts: ["dsp", "wavelets"]
equations:
  - 'y[n] = \sum_{k=-\infty}^{\infty} x[k]h[n-k]'
  - 'S_{xx}(\omega) = \int_{-\infty}^{\infty} R_{xx}(\tau)e^{-j\omega\tau} d\tau'
links:
  - "projects"
  - "dsp"
  - "stochastic"
  - "wavelets"
---

The analysis, synthesis, and modification of signals. My focus is on stochastic signal processing in high-noise environments and optimal estimation theory.

## Mathematical model

Convolution and spectral analysis describe how a linear system transforms an input signal in time and frequency. Estimation theory takes over from there, asking how to recover the true underlying signal when what you actually have is a noisy measurement of it.

## Implementation

A Kalman filter is the clearest example: at each sample, estimate the noise, subtract it, and update a running state estimate that folds in everything seen so far.

```python
def process_signal(input_vector):
    state = initialize_basis()
    for sample in input_vector:
        noise = estimate_noise(sample)
        filtered = sample - noise
        state = update_kalman(state, filtered)
    return state.optimal_estimate
```

## Where this goes

The interesting part isn't the filter itself but tuning it: getting the noise and process covariances right for a specific sensor is closer to fitting a statistical model than writing code.
