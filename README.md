# TESSERACT-NODE v1.0

## Overview
TESSERACT-NODE is an offline quantum server simulating 4D spacetime coordinates using Python. It leverages Qiskit for quantum circuit simulations (e.g., Bell pairs, GHZ states) and Flask for a local API. Runs on `127.0.0.1:8888` with background drift for dynamic positioning. Ideal for prototyping quantum concepts in a 4D framework.

## Features
- **4D Spacetime Simulation**: Track and move through 4D coordinates (ct, x, y, z).
- **Quantum Operations**: Generate entangled pairs and GHZ states via Qiskit AerSimulator.
- **HyperMemory Storage**: Store/retrieve data at 4D coordinates.
- **API Endpoints**:
  - `/status`: Node status and position.
  - `/entangle`: Create Bell pair.
  - `/ghz`: Generate 4-qubit GHZ state.
  - `/move`: Update position with dt/dx parameters.
- **Background Drift**: Automatic random movement every 10 seconds.

## Requirements
- Python 3.8+
- Libraries: `qiskit`, `qiskit-aer`, `flask`, `numpy`, `matplotlib`

Install via:
pip install qiskit qiskit-aer flask numpy matplotlib

## Usage
Run the script:

Access at `http://127.0.0.1:8888/`. Use browser or tools like curl for endpoints.

Example: `curl http://127.0.0.1:8888/entangle`

## License
MIT License. Copyright (c) Daniel Harding - RomanAILabs.

## Contributing
Fork, modify, PR. Issues welcome!
