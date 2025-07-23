# UART AXI4-Stream Interface | Verilog Project

This is my implementation of an **8-bit UART IP core** with an AXI4-Stream interface in Verilog, including transmitter and receiver modules, tested using cocotb-based Python testbenches.

---

## Features

- UART transmitter and receiver with **configurable data width (default 8 bits)**
- Supports **runtime configurable baud rate** via prescaler input
- Implements **start and stop bit framing logic**
- AXI4-Stream compliant interface for integration with other IPs
- Includes **functional testbenches** for both TX and RX

---

## Folder Structure

```
rtl/        --> Verilog design files (uart.v, uart_tx.v, uart_rx.v)
tb/         --> cocotb testbenches for transmitter and receiver
```

---

## Running Simulations

### Prerequisites

- Python with `cocotb`, `cocotb-test`, and `cocotbext-axi`
- Icarus Verilog
- GTKWave (for waveform viewing)

### Steps

```bash
# Clone the repository
git clone https://github.com/yourusername/UART_AXI4.git
cd UART_AXI4

# (Optional) Create virtual environment
python -m venv uartenv
source uartenv/bin/activate

# Install dependencies
pip install cocotb cocotb-test cocotbext-axi

# Set PYTHONPATH to tb folder
export PYTHONPATH=tb

# Run tests using pytest
pytest tb/
```

> **Note:** Use `gtkwave dump.vcd` to view waveform outputs for each test.

---

## Learning Objectives

- Designing AXI4-Stream compliant interfaces in Verilog
- Implementing UART protocols with start/stop framing logic
- Writing cocotb-based Python testbenches for IP verification
- Debugging simulation waveforms to validate functionality

---

## Author

- Name : Dhakshith Sureshkumar
- Roll Number : 230359
- B.Tech in Electrical Engineering
