# bus-scanner
A practical web app utility developed by Bartlett UCL Connected Environments for scanning student ID card barcodes and saving a timestamped list of codes in a CSV file.

## Overview
ScannerPro (Bus Scanner) is a single-page HTML5 application that utilizes the device's camera to scan barcodes. It processes both 1D and 2D barcodes seamlessly using the `html5-qrcode` library.

### Key Features
- **Camera Integration**: Direct access to the device camera for fast scanning without needing external apps, optimized for wide 1D barcodes.
- **Local Storage**: Scanned barcodes are automatically saved to your browser's local storage (`localStorage`), allowing you to close the page and return later without losing data.
- **Audio Feedback**: Plays a beep sound upon successful scan.
- **Deduplication**: Prevents accidental duplicate consecutive scans within a 3-second window.
- **Export to CSV**: Easily download all accumulated scan records as a CSV file for further processing. You can see an example output here: [scans_2026-02-28.csv](./scans_2026-02-28.csv).
- **Data Management**: Delete individual scans or clear all saved data completely.
