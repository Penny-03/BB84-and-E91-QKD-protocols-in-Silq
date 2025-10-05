# BB84 and E91 Quantum Key Distribution (QKD) in Silq

This repository contains implementations and simulations of the **BB84** and **E91** Quantum Key Distribution (QKD) protocols using **Silq**, a high-level quantum programming language.

The goal of this project is to provide both **educational** and **practical** insights into quantum cryptography:

* **BB84 Protocol**: Demonstrates key exchange using polarized qubits, including eavesdropping detection.
* **E91 Protocol**: Implements an entanglement-based QKD protocol and calculates CHSH correlations to verify security.

Three versions of the code are provided for the BB84 protocol:

* **Slow but clear version**: Prioritizes readability to help understand how the protocol works.
* **Efficient version**: Optimized for performance, but less intuitive for learning purposes.
* **Efficient version with Eve**: You can choose whether to include Eve by changing the `eve_present` flag, and set the percentage of intercepted qubits using `p_eve` in the main function.

There is one version for the E91 protocol where you can choose to include Eve using the `with_eve` flag and set the attack probability in `def main()`.  
Example:
```python
def main():
    print(E91_protocol(0.0))  # Run the protocol with 0% attack probability
```
## Features

* Simulate qubit transmission and measurement.
* Analyze the effects of eavesdropping on key security.
* Calculate the qubit error rate to check BB84 security.
* Calculate CHSH S-values for E91 to verify quantum correlations.

## Requirements

* [Silq](https://silq.ethz.ch/) 
* Python 3.x (for running auxiliary scripts and simulations)



