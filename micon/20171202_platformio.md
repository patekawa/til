# Basic usage for PlatformIO

## What is "PlatformIO"

[PlatformIO](http://platformio.org/) is a cross-platform development framework for IoT devices.

## Requirements

- Python2.7

When you install PlatformIO or build a project, other requirements will be installed automatically.

## Installation

Only run the command `pip install platformio`!

## usage

### Create a project

To see a list of supported boards, run `platformio boards`.
You can use `pio` command instead of `platformio`.

The example above uses `Arduino UNO` board.

To create a project in a directory, you run
```
platformio init --board uno
```
You can specify multiple boards in ``--board`` option.

### Create source codes

Make source codes in `src` directory.

### Build a project

To build a project, you run the command below in the project directory.
```
platformio run
```

### Upload a binary to a board

To upload a program to a board, you run the command below;
```
platformio run --target upload --upload-port /dev/ttyS5
```
where the board is connected to `/dev/ttyS5`.
