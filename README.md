# Boolean Quantum Circuit Simulation

This Jupyter notebook demonstrates the implementation of classical Boolean logic gates and digital circuits using quantum computing principles with Qiskit.

## Overview

The notebook provides quantum circuit implementations of fundamental logic gates and digital components:

- NOT Gate (X Gate)
- XOR Gate (CNOT Gate)
- AND Gate (Toffoli Gate)
- OR Gate
- NAND Gate
- NOR Gate
- Full Adder Circuit
- 1-Bit Comparator (A > B)

## Prerequisites

To run this notebook, you'll need:

- Python 3.x
- Qiskit
- Matplotlib
- NumPy

```bash
pip install qiskit matplotlib numpy
```

## Implementation Details

Each logic gate/circuit follows a similar pattern:

1. Initialize quantum and classical registers
2. Set input states using the `initialize` method
3. Apply quantum gates to implement the desired logic
4. Measure the output register(s)
5. Run the simulation using `AerSimulator`
6. Display the circuit diagram and histogram of measurement results

## Gate Implementations

### NOT Gate
Implements logical negation using the Pauli-X gate (quantum equivalent of classical NOT gate).

### XOR Gate
Implements exclusive-OR using the CNOT (controlled-X) gate.

### AND Gate
Implements logical AND using the Toffoli (CCNOT) gate.

### OR Gate
Implements logical OR using X gates and a Toffoli gate.

### NAND Gate
Implements logical NAND (NOT-AND) using a Toffoli gate followed by an X gate.

### NOR Gate
Implements logical NOR (NOT-OR) using X gates and a Toffoli gate.

### Full Adder
Implements a 1-bit full adder with carry-in and carry-out:
- Inputs: A, B, Cin
- Outputs: Sum (A ⊕ B ⊕ Cin), Cout

### 1-Bit Comparator
Implements a 1-bit comparator checking if A > B.

## Usage

Each section of the notebook runs a simulation for all possible input combinations and displays:
1. The quantum circuit diagram
2. A histogram showing the measurement outcomes
3. Text output confirming the truth table values

## Results

All simulations run with 1024 shots and consistently show 100% accuracy, demonstrating the deterministic nature of these quantum implementations of classical logic.

## Educational Value

This notebook serves as an excellent introduction to:
- Quantum circuit design principles
- Quantum gate operations
- Quantum computing's relationship to classical computation
- Qiskit's simulation capabilities

## Future Extensions

Possible extensions to this notebook could include:
- Multi-bit arithmetic circuits
- Quantum multiplexers and decoders
- Sequential logic elements (flip-flops, registers)
- More complex ALU components

## References

- [Qiskit Documentation](https://qiskit.org/documentation/)
- [Quantum Computing: An Introduction](https://quantum-computing.ibm.com/)
- [Boolean Logic Gates in Quantum Computing](https://qiskit.org/textbook/ch-states/atoms-computation.html)
