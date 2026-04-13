## Pauli Z Operator
Pauli Z or just 'Z' operator is a phase flip operator. It flips the phase if qubit is in |1> state and does nothing if is in state |0>
Imports

    from qiskit.quantum_info import Operator, Statevector
    from qiskit import QuantumCircuit, QuantumRegister

Define
      
    Z = Operator([[1, 0],[0, -1]])
      
Matrix representation

    Z.draw("latex")
      
<kbd><img width="67" height="50" alt="image" src="https://github.com/user-attachments/assets/f2fb0224-7eee-427b-986d-25e52aee9770" /></kbd>

## Pauli Z on QuantumCircuit
Define Quantum Ciruit
      
    zdemo = QuantumRegister(1, "Q1")
    qc = QuantumCircuit(zdemo)
    qc.draw("mpl")
<kbd><img width="156" height="122" alt="image" src="https://github.com/user-attachments/assets/f982328d-32e2-43a3-9ea6-3e1b0f410620" /></kbd>

Look at state

    Statevector.from_circuit(qc).draw("latex")

<kbd><img width="26" height="26" alt="image" src="https://github.com/user-attachments/assets/2b67b11c-44a3-406c-bed5-c378c0e9b020" /></kbd>

Apply Pauli Z on Qubit 1

    qc.z(zdemo)
    qc.draw("mpl")

<kbd><img width="191" height="120" alt="image" src="https://github.com/user-attachments/assets/8bb1b993-90df-4007-85f1-d21193b25bd0" /></kbd>

State after Pauli Z is applied

<kbd><img width="26" height="26" alt="image" src="https://github.com/user-attachments/assets/2b67b11c-44a3-406c-bed5-c378c0e9b020" /></kbd>

Pauli Z, flips the phase if qubit is in |1> state and does nothing if is in state |0>

<kbd><img width="104" height="60" alt="image" src="https://github.com/user-attachments/assets/90568665-5ea6-472f-80a1-bbbeae5b8b69" /></kbd>
