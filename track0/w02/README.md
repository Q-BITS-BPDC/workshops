# W02 — Quantum Gates 101

**Track:** 0 — Foundations  
**Prerequisites:** W01  
**Duration:** ~60 minutes

---

## Overview

Quantum gates are the operations we apply to qubits — the quantum equivalent of classical logic gates. Unlike classical gates, all quantum gates are **reversible** and represented by **unitary matrices**. This workshop covers the most important single-qubit and two-qubit gates, how to compose them into circuits, and how to reason about what they do geometrically.

By the end of this session you will be able to:
- Explain why quantum gates must be unitary
- Apply and interpret the X, H, Z, S, and T gates
- Understand and construct the CNOT gate
- Compose multi-gate circuits in Qiskit
- Read and draw circuit diagrams

---

## Topics Covered

- Unitary matrices and why gates must be reversible
- Single-qubit gates: X (NOT), Z, H (Hadamard), S, T
- Gate action on the Bloch sphere
- Two-qubit gates: CNOT (CX)
- Circuit composition and gate order
- Identity and inverse gates
- Circuit diagrams in Qiskit

---

## Materials

| File | Description |
|---|---|
| `notebook.ipynb` | Hands-on notebook — theory interleaved with code |
| `slides.pdf` | Session slides |

---

## Further Reading

- [IBM Quantum Learning — Single Qubit Gates](https://learning.quantum.ibm.com/course/basics-of-quantum-information/single-systems#unitary-operations)
- Nielsen & Chuang, Chapter 1.3 — *Single qubit operations*
- [Quirk](https://algassert.com/quirk) — drag-and-drop gates, instant visual feedback

---

**Previous:** [W01 — What is a Qubit?](../W01/)  
**Next:** [W03 — Your First Circuit](../W03/)
