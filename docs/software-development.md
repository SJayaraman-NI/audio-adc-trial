# Setup a Development Environment
If you want to commit changes to the repo, we recommend you use the current versions of application software unless a newer version enables new features. Software should work with newer versions of these dependencies.

## Software dependencies:
Install the below softwares and packages from NIPM

- NI-DAQmx (2022 Q3 or higher)
- NI-Digital Audio Acquisition and Generation Toolkit (2023 Q3 or higher)
- NI-DCPower (2023 Q1 or version as recommended by Instrument Studio)
- LabVIEW Sound and Vibration Toolkit (2021 or higher)
- LabVIEW Runtime Engine (2021 SP1 or higher)
- LabVIEW 64-bit (2021 SP1 or higher)
- InstrumentStudio (2023 Q3 or higher)
- Measurement Link (2023 Q3 or higher)

## VIPM packages
Install the following .vip files in the same order mentioned below

- Grpc library
- Grpc servicer
- Measurement link service
- Measurement link generator

The files can be found located at https://github.com/ni/measurementlink-labview/releases/tag/v1.0.1

Tested with:
- Instrument Studio 2023 Q1
- TestStand 2023 Q4

## Github and LabVIEW Guidelines:
Refer to [this](github-labview-guidelines.md) document for guidelines on github processes and labview development.

## Building NIPM packages
To build NIPM packages for the measurement plugin, refer to the [this](build-meas-package.md) document.