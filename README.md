# Introduction to Qiskit
![Quantum Machine](https://github.com/arcesoftware/Qiskit/blob/main/quantum_machine.png)
The name "Qiskit" refers to a collection of software tools for executing programs on quantum computers. Most notably among these tools are:

- The **open-source Qiskit SDK**, and
- The **runtime environment** (accessed using Qiskit Runtime) for executing workloads on IBM® quantum processing units (QPUs). 

As quantum technology evolves, so does Qiskit, with new capabilities released every year to expand this core collection of quantum software.

In addition, many open-source projects are part of the broader Qiskit ecosystem. These tools are not part of Qiskit itself but interface with Qiskit to provide valuable additional functionality.

## The Qiskit Workflow
Qiskit encompasses all steps of the quantum computation process:
1. **Map the problem** 
2. **Optimize for hardware** 
3. **Execute on hardware** 
4. **Post-process results**

- All steps, except for 'Execute on hardware,' use the Qiskit SDK. 
- 'Optimizing for hardware' additionally uses the Qiskit Transpiler Service. 
- 'Executing on hardware' relies on the Qiskit Runtime Service.

IBM is committed to the responsible development of quantum computing. Learn more about IBM's responsible quantum principles in the **[Responsible quantum computing](https://www.ibm.com/quantum/what-is-quantum-computing/responsible-quantum)** topic.

---

## The Qiskit SDK

The **Qiskit SDK** (package name: `qiskit`) is an open-source toolkit for working with quantum computers. It provides tools for extended (static, dynamic, and scheduled) quantum circuits, operators, and primitives. As the largest and most comprehensive Qiskit package, it serves as the core component of the Qiskit ecosystem. Other components interface seamlessly with the SDK.

### Features of the Qiskit SDK:
- **Circuit-building tools (`qiskit.circuit`)**  
  For initializing and manipulating registers, circuits, instructions, gates, parameters, and control flow objects.

- **Circuit library (`qiskit.circuit.library`)**  
  A vast range of circuits, instructions, and gates—key building blocks for circuit-based quantum computations.

- **Quantum info library (`qiskit.quantum_info`)**  
  A toolkit for working with quantum states, operators, and channels using exact calculations (no sampling noise). This module is useful for specifying input observables and analyzing output fidelity from primitives queries.

- **Transpiler (`qiskit.transpiler`)**  
  For transforming and adapting quantum circuits to suit specific device topology and optimizing for execution on real quantum processing units (QPUs).

- **Primitives (`qiskit.primitives`)**  
  Contains the base definitions and reference implementations of the Sampler and Estimator primitives. Hardware providers can derive their implementations from these primitives. For more information, refer to the **[Qiskit Runtime primitives documentation](https://qiskit.org/documentation/)**.

---

## Installation

For detailed installation instructions, visit the **[Qiskit SDK installation page](https://qiskit.org/documentation/install.html)**. 

If you're ready to install now, simply run:

```bash
pip install qiskit
```

# The Qiskit Ecosystem

Beyond the core Qiskit SDK, the Qiskit ecosystem includes numerous open-source projects that use the "Qiskit" name but are not part of Qiskit itself. These projects interface with Qiskit to provide valuable additional functionality that supplements the core Qiskit workflow. 

Some of these projects are maintained by IBM Quantum teams, while others are supported by the broader open-source community. The Qiskit SDK is designed in a modular, extensible way, enabling developers to create projects that extend its capabilities.

## Popular Projects in the Qiskit Ecosystem

### 1. **Qiskit Aer (`qiskit-aer`)**
- A package for quantum computing simulators with realistic noise models.
- Provides interfaces to run quantum circuits with or without noise using multiple simulation methods.
- **Maintained by:** IBM Quantum.

### 2. **qBraid SDK (`qbraid`)**
- A platform-agnostic quantum runtime framework designed for quantum software and hardware providers.
- Streamlines the full lifecycle of quantum jobs—from defining program specifications, job submission, to post-processing and visualization of results.
- **Maintained by:** qBraid.

### 3. **Mthree (`mthree`)**
- Implements M3 (Matrix-free Measurement Mitigation), a technique for correcting measurement probabilities.
- Uses a dimensionality reduction step followed by direct LU factorization or a preconditioned iterative method. These methods nominally converge in \( O(1) \) steps and can compute in parallel.
- **Maintained by:** IBM Quantum.

---

## Explore More

You can discover additional projects in the **[Qiskit ecosystem catalog](https://qiskit.org/ecosystem)**. This catalog also provides guidance on how to nominate your own project to become part of the Qiskit ecosystem.

 **Maple Software 2025 by John Maple** 

