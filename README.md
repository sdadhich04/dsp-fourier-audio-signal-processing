# Fourier and Audio Signal Processing

Eight Jupyter notebooks from an EE 242 signal-processing lab sequence. They work with sampled signals and WAV audio to illustrate time-domain operations, convolution, Fourier analysis, and digital filtering.

## What the notebooks cover

- Resampling, time scaling, time reversal, and amplitude changes for audio signals.
- Convolution of simple discrete-time signals and moving-average smoothing of synthetic and noisy trombone signals.
- Fourier-series synthesis of sawtooth and triangle waves, plus a short horn-note approximation.
- DFT/FFT plots for a horn segment and selected speech-sound windows.
- FIR and Butterworth filter response, impulse-response, and smoothing comparisons.

## Tools and hardware

The notebooks use Python with NumPy, SciPy, Matplotlib, and IPython. They are intended for Jupyter notebooks. No dedicated hardware requirement is documented in the tracked files.

## Run

Install the listed Python dependencies:

```bash
python -m pip install -r requirements.txt
```

Open a notebook with Jupyter (install it separately if it is not already available):

```bash
python -m pip install jupyter
jupyter notebook
```

The repository does not include WAV inputs. Audio cells expect files such as `baby.wav`, `train32.wav`, `trombone11.wav`, `horn11short.wav`, and `bluenose3.wav` beside the notebook that uses them. Generated audio is ignored by Git.

## Notes

- Lab 1b's time-shift exercise is incomplete; its `timeshift` cell contains `n_0 = ;`.
- `lab1a`, `lab2a`, `lab2b`, and `lab4` are marked in their notebooks as transcriptions from archived rendered views; those notebooks may contain compacted or clipped source lines.

## Credits

The notebooks identify Team AF07: Hanlin Ma, Amanda Zhang, and Sparsh Dadhich. Lab 0 identifies Hanlin Ma and Sparsh Dadhich.

No open-source license is granted; see [LICENSE](LICENSE).
