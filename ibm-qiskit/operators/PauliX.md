## Pauli X Operator
Pauli X or just 'X' operator is bit flip operator that flips the state of the qubit.
Imports

    from qiskit.quantum_info import Operator, Statevector
    from qiskit import QuantumCircuit, QuantumRegister

Define
      
    X = Operator([[0, 1],[1, 0]])
      
Matrix representation

    X.draw("latex")
      
<kbd><img width="78" height="66" alt="image" src="https://github.com/user-attachments/assets/9630b1da-5489-41e8-b188-f9cd053e049a" /></kbd>

## Pauli X on QuantumCircuit
Define Quantum Ciruit
      
    xdemo = QuantumRegister(1, "Q1")
    qc = QuantumCircuit(xdemo)
    qc.draw("mpl")
<kbd><img width="213" height="162" alt="image" src="https://github.com/user-attachments/assets/4e748990-6839-46cd-815e-0a28597853e6" /></kbd>

Look at state

    Statevector.from_circuit(qc).draw("latex")

<kbd><img width="35" height="37" alt="image" src="https://github.com/user-attachments/assets/177d208c-bcd9-4295-979c-08837f0c0bd6" /></kbd>

Apply Pauli X on Qubit 1

    qc.x(xdemo)
    qc.draw("mpl")

<kbd><img width="241" height="152" alt="image" src="https://github.com/user-attachments/assets/27664957-e819-4e1e-9218-8ae6aca97781" /></kbd>

State after Pauli X is applied

<kbd><img width="37" height="38" alt="image" src="https://github.com/user-attachments/assets/fabb0b50-8883-4ba0-9a7f-0d701856043f" /></kbd>

Pauli X, flips the state of the qubit, from |0> to |1> and vice versa.
