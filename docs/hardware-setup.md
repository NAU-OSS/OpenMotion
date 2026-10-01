# Hardware Setup

This guide explains how to assemble and configure a basic OpenMotion hardware setup for collecting motion data.

OpenMotion is designed to work with affordable microcontrollers and inertial measurement units (IMUs). The initial reference platform is the Arduino Nano 33 BLE Rev2, which includes an onboard accelerometer, gyroscope, and magnetometer.

## Supported Hardware

The initial reference hardware is:

- Arduino Nano 33 BLE Rev2

This board is suitable for OpenMotion because it includes:

- Accelerometer
- Gyroscope
- Magnetometer
- USB connectivity
- Built-in microcontroller

Other microcontrollers and external IMUs may be supported in the future.

## Required Components

For the reference setup, you will need:

- Arduino Nano 33 BLE Rev2
- USB cable compatible with the board
- Computer running Windows, macOS, or Linux
- Arduino IDE or Arduino CLI

Because the Nano 33 BLE Rev2 contains onboard motion sensors, no external IMU or additional wiring is required for the basic setup.

## Connections

For the reference platform:

1. Connect the Arduino Nano 33 BLE Rev2 to the computer using USB.
2. Verify that the computer detects the board.
3. Select the correct serial port in the Arduino development environment.

No external sensor wiring is required when using the onboard IMU.

## Microcontroller Setup

1. Install the Arduino IDE or Arduino CLI.
2. Connect the Arduino Nano 33 BLE Rev2 using USB.
3. Install the board support package for the Nano 33 BLE Rev2.
4. Select the correct board and serial port.
5. Upload the OpenMotion firmware when firmware becomes available in the project.

## IMU Configuration

The Arduino Nano 33 BLE Rev2 includes onboard motion sensors.

The OpenMotion firmware is expected to read measurements such as:

- Acceleration
- Angular velocity
- Magnetic field data

Sensor configuration such as sampling rate and calibration may depend on the firmware implementation.

## Required Software

A basic OpenMotion setup may require:

- Arduino IDE or Arduino CLI
- OpenMotion firmware
- Serial communication support
- OpenMotion data collection tools

The project is currently in early development, so some software components may not yet be available.

## Basic Troubleshooting

### Board is not detected

- Reconnect the USB cable.
- Try another USB port.
- Verify that the cable supports data transfer.
- Check that the correct board support package is installed.

### Serial port does not appear

- Disconnect and reconnect the board.
- Restart the Arduino IDE.
- Verify that the operating system detects the device.

### No sensor data is received

- Confirm that firmware has been uploaded successfully.
- Confirm that the correct serial port is selected.
- Restart the board.
- Verify that the firmware supports the onboard IMU.

## Example Data Collection Procedure

A typical OpenMotion data collection workflow is expected to be:

1. Connect the Arduino Nano 33 BLE Rev2 to the computer.
2. Upload the OpenMotion firmware.
3. Start the OpenMotion data collection software.
4. Select the correct serial connection.
5. Begin recording.
6. Move or rotate the board to generate motion data.
7. Stop recording.
8. Save the recorded dataset.
9. Load the dataset for visualization or analysis.

## Project Status

OpenMotion is currently in the planning and early development stage.

Some setup steps may change as firmware, data collection tools, and additional hardware support are added.
