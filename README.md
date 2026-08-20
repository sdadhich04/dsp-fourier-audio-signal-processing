# Fourier and Audio Signal Processing

Post-course portfolio curation of eight EE 242 lab notebooks from University of
Washington ECE, Winter 2025. The work follows one DSP progression across the
quarter: sampling, time-domain operations, convolution, denoising, Fourier
series synthesis, FFT analysis, and digital filter design on audio signals.

This was collaborative coursework by Team AF07. Lab 0 names Hanlin Ma and
Sparsh Dadhich; Labs 1a through 4 name Hanlin Ma, Amanda Zhang, and Sparsh
Dadhich. This repository was curated after the course for portfolio review.

## Publication Status

Keep this repository private unless the following are resolved:

- Collaborator credit and permission for public portfolio use.
- UW/course permission for publishing notebooks that still include lab prompt
  markdown and starter-context text.
- Replacement or removal of course-distributed audio files. The audio files are
  intentionally not bundled here.

The code has been lightly curated for local reproducibility and privacy:
machine-specific absolute audio paths were changed to relative filenames, and
saved notebook outputs were cleared. The unfinished lab sections were not
completed after the course.

## Repository Contents

| Folder | Topic | Notes |
| --- | --- | --- |
| `lab0` | Python and audio warm-up | Palindrome and vowel-cipher exercises are implemented. The audio exercise is only a comment template. |
| `lab1a` | Sampling-rate resampling | Reconstructed notebook. Compares polyphase and linear resampling on train audio. |
| `lab1b` | Time scaling and time shift | Time scaling is implemented. The time-shift exercise is genuinely incomplete and contains a syntax error. |
| `lab2a` | Convolution basics | Builds simple signals and compares smoothing and differencing convolutions. |
| `lab2b` | Convolution denoising | Reconstructed notebook. Smooths synthetic noise and noisy trombone audio with a box filter. |
| `lab3a` | Fourier series synthesis | Reconstructs sawtooth/triangle waves and synthesizes a horn note from Fourier coefficients. |
| `lab3b` | FFT analysis | Compares 1024/2048-point FFTs and analyzes selected speech phoneme windows. |
| `lab4` | Digital filter design | Reconstructed notebook. Compares FIR and Butterworth filters and analyzes a moving-average lowpass. |

## Provenance

Four notebooks were reconstructed from archived rendered notebook/PDF views
because local `.ipynb` files were unavailable:

- `lab1a/EE242_Lab1a_transcribed.ipynb`
- `lab2a/EE242_Lab2a_transcribed.ipynb`
- `lab2b/EE242_Lab2b_transcribed.ipynb`
- `lab4/EE242_Lab4_transcribed.ipynb`

The remaining notebooks are local notebook files from the course archive:

- `lab0/EE242_Lab0.ipynb`
- `lab1b/EE242_Lab1b.ipynb`
- `lab3a/EE242_Lab3a.ipynb`
- `lab3b/EE242_Lab3b.ipynb`

## Data Policy

No `.wav` files are committed. The notebooks expect these audio files beside the
notebook that uses them:

- `baby.wav`
- `train32.wav`
- `trombone11.wav`
- `horn11short.wav`
- `bluenose3.wav`

Generated audio such as `slow.wav`, `fast.wav`, `reverse.wav`, `tr_noisy.wav`,
and `tr_filt.wav` is also ignored.

## Known Limitations

- `lab0` exercise 0.3 is not implemented; its code cell contains comments only.
- `lab1b` Assignment 4 is not implemented; the `timeshift` function contains
  `n_0 = ;` and the remaining parts are placeholders.
- Reconstructed notebooks may still contain clipped or compacted lines from the
  archived rendering source.
- Dependencies are unpinned because the original environment was not captured.

## Running

Install the Python packages:

```bash
pip install -r requirements.txt
```

Open the notebooks in Jupyter or VS Code. To run audio cells, provide the
required `.wav` files in the relevant lab folder.

## License

No open-source license is granted at this time. See `LICENSE`.
