# INAV PID Optimizer GUI

This is a standalone GUI application for optimizing PID values from INAV blackbox CSV logs.

## Usage

1. Run `inav_pid_optimizer_gui.exe`
2. Click "Select CSV Files" to choose your decoded blackbox CSV files (.01.csv)
3. Click "Run Optimization" to analyze the logs
4. Review the optimized PID values in the output area
5. Apply the suggested values to your INAV configuration

## Features

- Analyzes multiple CSV files for stable flight characteristics
- Computes optimized P, I, D, and FF gains for Roll, Pitch, and Yaw
- Provides confidence levels and detailed metrics
- Outputs INAV CLI commands for easy application

## Requirements

- Windows 7 or later
- Decoded blackbox CSV files (use the Blackbox Decode GUI to create these)
- No additional software required (fully standalone)

## Notes

- Apply PID changes incrementally
- Re-log flights after changes
- Verify motor temperatures remain acceptable
- Zero error is not physically achievable

## Original Tool

Based on the INAV analyze_pids.py script.