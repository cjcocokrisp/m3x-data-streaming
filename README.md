# M3X Data Streaming

## Overview

This repository contains the data streaming code and datasets for the M3X project. Data streaming is done through a wrapper class that interacts with the Myopro 2 device through serial connections. The wrapper has functions for streaming data, changing the device's control parameters, and running commands that are not implemented. 

The library also allows for communication with Measurement Computing devices to be used with the Myopro 2 to collect extra information through the `mcculw` library.

## Installation

Installing this library is simple. Just download the code from this directory as a zip and then place the `myopro` folder in your project. 

There also are a few dependencies for the library being [`pyserial`](https://pypi.org/project/pyserial/) and [`mcculw`](https://github.com/mccdaq/mcculw). You can install them manually or use the `requirements.txt` file in the following manner.
```
pip install -r requirements.txt
```

## Usage 

To use the wrapper import the class by doing the following.
```
import myopro 
# or
from myopro import Device
```

There is also a starter code file called `starter.py`. This file contains some boilerplate code for connecting to the device that will be used whenever you are using the library.

## Documentation

The current functions provide doc strings that explain the functions arguments and usage. More detailed docs are currently being developed.

### Examples

There are some example files in the base directory when the project is installed. These examples can help you get started with usage of the code.

Current Examples:

- `example_change_control_parameter.py` - demonstrates how to change the control parameters of the device with the library.
- `example_daq.py` - shows how to use a Measurement Computing device with the code and read values from it.
- `example_real_time.py` - shows how to read the real time values of the device.
- `example_straming.py` - shows how to stream data from the devices.
- `example_streaming_2.py` - shows how to stream data from the devices using the `stream_data` method and explains the various arguments the function has.

## Datasets

The dataset directory contains various datasets collected for the project. 

Each dataset contains a README file that describes the overview of the dataset, the tasks preformed in it, and the sensors that data was collected from in that dataset.

Included Datasets:
- Data from Amin Majdi's expirements (`datasets/data_Amin`)
- Data from *Design of Fuzzy Logic Parameter Tuners for Upper-Limb Assistive Robots* UR 2024 WIP Paper (`datasets/data_Christopher_fuzzy_testing_jan_2024`)
- Data from *Investigating the Generalizability of Assistive Robots Models over Various Tasks* UR 2024 Paper (`datasets/data_Hamid_dec_2023`)
- Data that was used in various testing from things before the UR 2024 WIP Paper (`datasets/data_Christopher_random`)

## Publications

Christopher Coco, Jonathan Spanos, Hamid Osooli, Reza Azadeh, **"Design of Fuzzy Logic Parameter Tuners for Upper-Limb Assistive Robots,"**  *WIP paper at 21st International Conference on Ubiquitous Robots (UR)*, New York, USA, pp. 386--389, June 24-27, 2024. \[[arXiv](https://arxiv.org/pdf/2405.02495)\] \[[Video](https://www.youtube.com/watch?v=yRiI4b3mBeQ&feature=youtu.be)\] [Best WIP Paper Award Finalist]

Hamid Osooli, Christopher Coco, Jonathan Spanos, Amin Majdi, Reza Azadeh, **"Investigating the Generalizability of Assistive Robots Models over Various Tasks,"** *In Proc. 21st International Conference on Ubiquitous Robots (UR)*, New York, USA, pp. 227--232, June 24-27, 2024. \[[arXiv](https://arxiv.org/pdf/2405.02492)\]

## Contributors

Christopher Coco

Hamid Osooli

Amin Majdi

Jonathan Spanos

Reza Azadeh

## Questions and Issues

If you encounter any issues with the repository and/or its contents please open an issue!