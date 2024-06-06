# Dysarthria Speech Analysis

This repository contains scripts for extracting and analyzing acoustic features from speech samples associated with dysarthria. The analysis includes computing formants, pitch, LPCC, wavelet coefficients, spectral envelope and details, spectral centroid, spectral bandwidth, zero-crossing rate, mel spectrograms, and intensity. The results are visualized and saved to CSV files for further study.

## Features Extracted

- **Formants:** Derived from Linear Predictive Coding (LPC) coefficients.
- **Pitch:** Calculated using PyDub.
- **LPCC:** Linear Predictive Cepstral Coefficients.
- **Wavelet Coefficients:** Decomposition using wavelets.
- **Spectral Envelope and Details:** Smoothed magnitude spectrum and details.
- **Spectral Centroid:** Center of mass of the spectrum.
- **Spectral Bandwidth:** Width of the spectrum.
- **Zero-Crossing Rate:** Rate of sign changes in the signal.
- **Mel Spectrograms:** Mel frequency spectrograms.
- **Intensity:** Root Mean Square (RMS) of the audio signal.

## Usage

1. **Loading and Filtering Data:**
    - Load CSV file containing paths to audio files and metadata.
    - Filter out non-existent files.

2. **Extracting Features:**
    - Run the scripts to compute various acoustic features.
    - Visualize the results with plots.

3. **Saving Results:**
    - The computed statistics are saved to CSV files.

## Dependencies

- `numpy`
- `pandas`
- `librosa`
- `matplotlib`
- `pywt`
- `pydub`
- `scipy`

## Running the Analysis

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/dysarthria-speech-analysis.git
    ```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the analysis script:
    ```bash
    python analyze_speech.py
    ```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
