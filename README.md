# Tire Pressure Predictor

A professional tool for racing passionates that predicts optimal cold tire pressures to achieve target hot pressures during a stint.

## Overview

Tire Pressure Predictor uses a ML model trained on real telemetry data to predict the cold tire pressures needed to reach your target hot pressures after a specified number of laps in a specific track.

Instead of relying on trial-and-error or simplified linear formulas, this tool provides data-driven predictions based on previous data.

## Features

- **ML-based predictions** - Trained on real telemetry data for accurate results
- **Multi-software** - Import data from all telemetry softwares: Motec/WinDarab/WinTAX etc
- **Track-specific analysis** - Accounts for track characteristics
- **Pressure trend visualization** - Charts showing pressure evolution over laps
- **Auto track detection** - Uses GPS to automatically select the nearest circuit
- **Race Simulation mode** - Suggests the bleed to adopt after formation laps based on hystoric runs
- **NO TPMS mode** - For vehicles without Tire Pressure Monitoring System, get predictions with input-output simplified model
- **Custom track support** - Add tracks not in the database with scaling coefficients based on tracks similarity
- **Thermal correction tables** - Fine-tune predictions based on ambient conditions

## Screenshots

### Main Prediction Screen
Set your target hot pressures, select the track and number of laps, and get recommended cold pressures with pressure trend charts.

![Main Screen](screenshots/app-main.png)

### Race Simulation - Grid Bleed Calculator
Plan your race strategy with thermal gain coefficients and bleed recommendations for the formation lap.

![Race Sim](screenshots/app-bleed.png)

### Data Processing
Import your telemetry data with automatic channel detection and mapping.

![Data Processing](screenshots/app-processing.png)

### Channel Mapping
Custom mapping for different telemetry formats and data sources.

![Channel Mapping](screenshots/app-setup.png)

## System Requirements

- **OS:** Windows 10/11 (64-bit)
- **RAM:** 4 GB minimum
- **Disk:** 200 MB free space

## Installation

1. Download the latest installer from [Releases](../../releases)
2. Run `Tire Pressure Predictor Setup X.X.X.exe`
3. Follow the installation wizard
4. Launch the app from the Start Menu or Desktop shortcut

## License

This software requires a license to use. To obtain a license:

1. Visit [tirepressurepredictor.com](https://tirepressurepredictor.com) *(or contact info below)*
2. Contact the developer to request a license key
3. Enter the license key when prompted in the app

## Contact

For license requests, support, or feedback:

- **Email:** lvillaengineering@gmail.com

## Changelog

### v2.2.0 (Latest)
- **Prediction History Tab**: Track and manage saved predictions over time with Excel-like grid layout
- **Save Predictions**: Store prediction setups with driver, event type (Race/Test), session name, tire condition
- **Export for Tyre Manager**: Generate clean text files with prediction data for easy communication
- **Verification Workflow**: Add actual hot pressures after sessions to compare with predictions
- **History Filtering**: Filter by track, driver, event type, session, and date range
- **Bulk Delete**: Delete all visible (filtered) predictions at once
- **History Preservation**: Prediction history preserved when deleting vehicle/tire pairs

### v2.1.6
- **Single Instance Lock**: Prevents multiple app instances from running simultaneously
- **Windows Defender Prompt**: Installer prompts for Windows Defender exclusions

### v2.1.5
- **Concatenated Runs Detection**: Auto-detects and rejects files with multiple runs concatenated
- **Multi-Format Archive Support**: Upload .zip, .rar, .7z, .tar, .gz archives
- **Track Layout Channel Mapping**: GPS track layout generator supports custom channel mapping

### v2.1.4
- **Plateau Calculation Robustness**: No longer requires all 4 wheels to have data on the same lap/run
- **Cross-Axle Mismatch Warning**: Detects when predicted pressures on same axle differ by >0.2 bar
- **Pressure Trend Charts**: Fixed lap count display when out-lap is merged with lap 1
- **Clear Data Reset**: Software Type now resets properly when clearing processed data

### v2.1.3
- **Open Processed Data**: "Open" button to quickly access processed CSV files in file explorer

### v2.1.2
- **Misplaced Beacon Fix**: Auto-merges short initial laps caused by misplaced beacons

### v2.1.1
- **Race Sim Dual Mode**: Forward (pressures → bleed) or Reverse (target bleed → pressures)
- **Export Debug Logs**: Added missing file patterns for complete diagnostics

### v2.1.0
- **Percentile Normalization (v6.5)**: Fixed artificial variability in MIN/MAX predictions
- **Track Parameter Scaling**: Intelligent pressure scaling for custom tracks
- **Track Relations Matrix**: Cross-track coefficient matrices for pressure prediction
- **Manual Reference Track Selection**: Choose which track to use as reference

### v2.0.x
- Named Settings System with import/export
- Auto-detection of telemetry software
- Multi-software support (WinTax4, WinDarab, MoTeC)
- Channel mapping enhancements

See in-app Version History for complete details

## Disclaimer

This tool is intended for sim racing and track day preparation. Predictions are based on historical data and may vary from actual results. Always verify tire pressures with professional equipment before racing.

---

*Tire Pressure Predictor is proprietary software. The source code is not publicly available.*
