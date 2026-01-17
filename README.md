# Simulation-Based-Validation-of-9-Qubit-Shor-Quantum-Error-Correction-Code
This paper presents a simulation-based study of the 9-qubit Shor quantum error correction code. Fault-tolerant logical operations, exhaustive single-qubit error recovery, and statevector validation are analyzed using Qiskit simulators under ideal and noisy conditions.

# Abstract

Quantum error correction (QEC) is a fundamental requirement for reliable quantum computation in the presence of noise and decoherence. Among early QEC schemes, the 9-qubit Shor code remains a canonical construction capable of correcting arbitrary single-qubit errors. In this paper, we present a simulation-based study of the Shor code focusing on (i) fault-tolerant logical operations, (ii) exhaustive single-qubit error recovery, and (iii) statevector-level verification of logical encoding. Using Qiskit-based simulators, including deterministic, shot-based, and statevector backends, we analyze recovery performance under injected Pauli X, Y, and Z errors across all physical qubits. Furthermore, we contrast ideal error correction behavior with noisy quantum execution using depolarizing noise models. The results demonstrate successful logical operation preservation and near-complete recovery from single-qubit errors, while also revealing structural vulnerabilities related to simplified syndrome extraction and logical-qubit measurement. This work provides an educational yet rigorous benchmark for understanding fault tolerance, logical operators, and noise effects in early quantum error correction codes.

# 1. Introduction

Quantum computers promise exponential advantages for certain classes of problems; however, their practical realization is severely constrained by decoherence, gate imperfections, and environmental noise. Unlike classical systems, quantum information cannot be directly copied due to the no-cloning theorem, necessitating specialized quantum error correction (QEC) strategies.

The Shor code, introduced as the first quantum error-correcting code, encodes a single logical qubit into nine physical qubits and protects against arbitrary single-qubit errors by combining bit-flip and phase-flip correction mechanisms. Although modern QEC research focuses on surface codes and low-density parity-check codes, the Shor code remains an essential pedagogical and conceptual foundation for fault-tolerant quantum computation.

This paper presents a comprehensive simulation-based analysis of the 9-qubit Shor code implemented using Qiskit. Unlike purely theoretical descriptions, we emphasize executable circuits, logical gate validation, exhaustive error injection, and statevector inspection. We also investigate the behavior of the encoded system under realistic noise models and compare ideal correction with noisy outcomes.

The contributions of this paper are threefold:

1. Fault-tolerant logical operation validation using a logical Pauli-X gate.
2. Exhaustive single-qubit error testing for all Pauli error types across all nine physical qubits.
3.Statevector and noise-based analysis, highlighting both ideal behavior and realistic deviations.



Exhaustive single-qubit error testing for all Pauli error types across all nine physical qubits.

Statevector and noise-based analysis, highlighting both ideal behavior and realistic deviations.
