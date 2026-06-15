## **Title: Algebraic Embedding of Pell Sequences within Dirac Vector Spaces**

### **Abstract**

This document formalizes the Omega T framework by establishing a rigorous mathematical bridge between discrete integer sequences (Pell and Lucas) and continuous Hilbert space mechanics. By defining a finite-dimensional state vector and an associated linear operator, the asymptotic expansion ratios of recurrence sequences are calculated utilizing standard Dirac inner products.

### **Methodology**

**1\. State Vector Mapping**  
Discrete elements of the Pell sequence $P\_n$ are mapped to a two-dimensional vector space. The quantum state $| \\psi\_n \\rangle$ at index $n$ is defined as:  
$$| \\psi\_n \\rangle \= \\begin{pmatrix} P\_n \\\\ P\_{n-1} \\end{pmatrix}$$  
**2\. Operator Formalism**  
The standard Pell recurrence relation, $P\_{n+1} \= 2P\_n \+ P\_{n-1}$, is expressed via a time-evolution operator $\\hat{T}$. This transfer matrix advances the state vector:  
$$\\hat{T} \= \\begin{pmatrix} 2 & 1 \\\\ 1 & 0 \\end{pmatrix}$$  
The state progression is linearly defined as $| \\psi\_{n+1} \\rangle \= \\hat{T} | \\psi\_n \\rangle$.

### **Results: Asymptotic Evaluation**

The Dirac inner product is utilized to evaluate the dominant eigenvalue of the system, which represents the asymptotic expansion ratio. For large $n$, the expectation value of the operator $\\hat{T}$ isolates the Silver Ratio:  
$$\\lim\_{n \\to \\infty} \\frac{\\langle \\psi\_n | \\hat{T} | \\psi\_n \\rangle}{\\langle \\psi\_n | \\psi\_n \\rangle} \= 1 \+ \\sqrt{2}$$

### **Conclusion**

This formulation resolves the domain mismatch between discrete number theory and quantum mechanics. The bra-ket notation functions as a valid matrix-algebraic structure for extracting deterministic asymptotic limits from recurrence equations, providing explicit mathematical utility for the inner product.

—-

### **Spectral Decomposition**

The foundational piece to complete your algebraic embedding is the **Eigendecomposition** of the transfer operator $\\hat{T}$. This bridges the step-by-step vector evolution to a closed-form expression, acting as the matrix-algebraic equivalent of Binet's formula.  
By extracting the eigenvalues $\\lambda\_1 \= 1 \+ \\sqrt{2}$ and $\\lambda\_2 \= 1 \- \\sqrt{2}$, the quantum state can be expressed as a superposition of the operator's eigenkets:  
$$|\\psi\_n\\rangle \= c\_1 \\lambda\_1^n |e\_1\\rangle \+ c\_2 \\lambda\_2^n |e\_2\\rangle$$

### **Non-Unitary System Dynamics**

A secondary conceptual gap is the nature of the operator. In standard Dirac mechanics, time-evolution operators are unitary, preserving state probability. Your operator $\\hat{T}$ is non-unitary and real-symmetric.  
This means your framework describes an amplifying system rather than a conserved quantum state. The "wavefunction" norm diverges to infinity, which is why your asymptotic evaluation correctly requires normalizing by $\\langle \\psi\_n | \\psi\_n \\rangle$ to isolate the dominant eigenstate.