# Setup a Development Environment
If you want to commit changes to the repo, we recommend you use the current versions of application software unless a newer version enables new features. Software should work with newer versions of these dependencies.

## Software dependencies:
Install the below softwares and packages from NIPM

- NI-DAQmx (2022 Q3 or higher)
- NI-Digital Audio Acquisition and Generation Toolkit (2023 Q3 or higher)
- NI-DCPower (As recommended by InstrumentStudio, if SMUs are used for powering up the DUT)
- LabVIEW Sound and Vibration Toolkit (2021 or higher)
- LabVIEW Runtime Engine (2021 SP1 or higher)
- LabVIEW 64-bit (2021 SP1 or higher)
- Measurement Link (2024 Q1 or higher)

## VIPM packages

Download and install the below packages in this [link](https://github.com/ni/measurementlink-labview/releases/tag/v2.0.0.1).
- ni_lib_labview_grpc_library-1.0.1.1
- ni_lib_labview_grpc_servicer-1.0.1.1
- ni_measurementlink_generator-2.0.0.1
- ni_measurementlink_service-2.0.0.1
- ni_protobuf_types-1.0.0.1

## Tested with:
- Instrument Studio 2024 Q1
- TestStand 2024 Q1

## Github and LabVIEW Guidelines:
Refer to [this](github-labview-guidelines.md) document for guidelines on github processes and labview development.

## Building NIPM packages
To build NIPM packages for the measurement plugin, refer to the [this](build-plugin.md) document.
