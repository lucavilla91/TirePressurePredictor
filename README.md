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

### v2.1.0
- Latest stable release
- See in-app version history for details

## Disclaimer

This tool is intended for sim racing and track day preparation. Predictions are based on historical data and may vary from actual results. Always verify tire pressures with professional equipment before racing.

---

*Tire Pressure Predictor is proprietary software. The source code is not publicly available.*
