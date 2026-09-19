# UART Implementation in FPGA

## Overview

This project focuses on the design and implementation of a Universal Asynchronous Receiver/Transmitter (UART) transceiver using **Verilog HDL** on an FPGA platform. The system enables asynchronous serial communication by converting parallel data into serial form for transmission and reconstructing the original data at the receiver.

The UART design includes a finite state machine (FSM)-based transmitter and receiver, baud rate timing control, and receiver sampling for reliable data recovery. A seven-segment display and onboard LEDs are used to visualize received data.

## Features

* UART transmitter and receiver implemented using Verilog HDL.
* Configurable clock-cycle timing for UART communication at **9600 baud** with a 50 MHz clock.
* FSM-based control for start, data, and stop bit handling.
* UART receiver with midpoint sampling for reliable data reception.
* Seven-segment display and LED-based data visualization.
* Functional verification through simulation testbenches.
* Hardware implementation and bidirectional communication between two FPGA boards.

## Project Structure

* `uart_tx.sv` – UART transmitter module.
* `uart_rx.sv` – UART receiver module.
* `seven_seg.sv` – Seven-segment display decoder.
* `uart_top.sv` – Top-level module integrating the UART system.
* `tb_uart.sv` – Testbench for simulation and functional verification.

## Hardware and Tools

* **HDL:** SystemVerilog / Verilog HDL
* **FPGA:** DE0-Nano FPGA development board
* **Simulation and Synthesis:** Intel Quartus Prime
* **Communication Protocol:** UART
* **Baud Rate:** 9600

## Verification

The design was verified through simulation by transmitting and receiving multiple bytes of data. It was subsequently implemented on FPGA hardware and tested using two FPGA boards, demonstrating successful bidirectional UART communication and correct data visualization.

## Learning Outcomes

This project provided practical experience in RTL design, finite state machines, serial communication protocols, FPGA implementation, timing control, simulation-based verification, and hardware debugging.
