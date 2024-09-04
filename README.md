# Nervous Activity Analyzer

## Overview

The Nervous Activity Analyzer is a MATLAB-based tool designed for digital filtering and analysis of raw EEG signals. This project allows users to load EEG data, apply digital filtering, extract different brainwave frequencies (alpha, beta, theta, delta), and compute statistical metrics such as standard deviation, average, and cross-correlation. The tool includes an interactive GUI for user-friendly operation.

## Features

- **Load EEG Data**: Load raw EEG data from a file.
- **Digital Filtering**: Apply FIR filters to remove noise and extract specific brainwave frequencies.
- **Brainwave Extraction**: Analyze and extract alpha, beta, theta, delta, and gamma brainwaves from the EEG signal.
- **Statistical Computations**: Compute standard deviation (STD), average (AVG), and cross-correlation (CC) of the EEG signal.
- **Interactive GUI**: Easy-to-use graphical user interface for parameter input and data visualization.

## GUI Components

- **Load EEG Button**: Load EEG data from a file and display the file path.
- **Filter Menu**: Toggle filter application on/off.
- **Wave Menu**: Select which brainwave frequency to analyze (Delta, Theta, Alpha, Beta, Gamma).
- **Column Input**: Specify the column in the data file containing EEG data.
- **Frequency Input**: Specify the sampling frequency of the EEG data.
- **Start Time and End Time Inputs**: Define the time range for analysis.
- **Compute Button**: Perform the data processing and analysis based on the provided parameters.
- **Results Display**: Show extracted wave type, standard deviation, average, and cross-correlation results.

## Installation

1. Ensure MATLAB is installed on your system.
2. Download the `BioProject1.fig` and `BioProject1.m` files.
3. Open MATLAB and navigate to the directory containing the files.
4. Run the command `BioProject1` in the MATLAB command window to start the GUI.

## Usage

1. **Load EEG Data**: Click the "Load EEG" button to select and load an EEG data file. The file path will be displayed in the GUI.
2. **Set Parameters**:
   - Enter the column number where the EEG data is stored.
   - Enter the sampling frequency of the EEG data.
   - Specify the start and end time for analysis.
   - Choose whether to apply filtering or not.
   - Select the brainwave frequency to analyze from the "Wave Menu".
3. **Compute**: Click the "Compute" button to process the data.
4. **View Results**:
   - The EEG signal and filtered signal will be plotted in the GUI.
   - Results for selected wave type, standard deviation, average, and cross-correlation will be displayed.

## Code Explanation

- **Filter Application**: FIR filters are used to remove noise and extract specific frequency bands.
- **Wave Extraction**: FFT and IFFT are used to transform the signal and isolate different brainwave frequencies.
- **Statistical Metrics**: Standard deviation, average, and cross-correlation are calculated and displayed based on the filtered signal.

## Notes

- Ensure the EEG data file is properly formatted with numerical values.
- The GUI requires proper input values for accurate results. Ensure all inputs are valid before computing.

