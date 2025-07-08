# ⚡ AXI4-Stream UART Implementation in Verilog

This project implements a **parameterizable 8-bit UART transmitter and receiver** with AXI4-Stream interfaces, enabling high-speed serial communication integration into FPGA designs.

---

## 📂 Modules

- `uart.v`: Top-level wrapper instantiating TX and RX modules
- `uart_tx.v`: UART transmitter implementation
- `uart_rx.v`: UART receiver implementation

---

## ⚙️ Features

- **AXI4-Stream interface** with `tdata`, `tvalid`, `tready` handshaking
- Configurable **DATA_WIDTH** and prescaler-based baud rate control
- Start and stop bit framing with framing and overrun error detection
- Synthesizable clean Verilog design with cocotb testbenches

---

## 🧪 Simulation Instructions

1. **Install dependencies**
   ```bash
   pip install cocotb cocotbext-axi pytest
