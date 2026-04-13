## Pauli Y Operator
Pauli Y or just 'Y' operator combines bit flip(Pauli X) and phase flip(Pauli Z) upto global phase.
Imports

    from qiskit.quantum_info import Operator, Statevector
    from qiskit import QuantumCircuit, QuantumRegister

Define
      
    Y = Operator([[0, -1.0j],[1.0j, 0]])
      
Matrix representation

    Y.draw("latex")
      
<kbd><img width="67" height="51" alt="image" src="https://github.com/user-attachments/assets/23cf2b08-8c53-4ccc-8277-f50395dca61c" /></kbd>

## Pauli Y on QuantumCircuit
Define Quantum Ciruit
      
    ydemo = QuantumRegister(1, "Q1")
    qc = QuantumCircuit(ydemo)
    qc.draw("mpl")
    
<kbd><img width="163" height="124" alt="image" src="https://github.com/user-attachments/assets/c58eed39-d8da-4871-ba61-76ef6fd23427" /></kbd>

Look at state

    Statevector.from_circuit(qc).draw("latex")

<kbd><img width="28" height="29" alt="image" src="https://github.com/user-attachments/assets/1faa4890-4386-44db-941f-b4931fc735cd" /></kbd>

Apply Pauli Y on Qubit 1

    qc.y(ydemo)
    qc.draw("mpl")

<kbd><img width="192" height="123" alt="image" src="https://github.com/user-attachments/assets/7545790d-d6b7-46b4-b180-ae8a610b2654" /></kbd>

State after Pauli Y is applied

<kbd><img width="37" height="30" alt="image" src="https://github.com/user-attachments/assets/f88a0cc7-10a9-4a2d-9251-ee979eedaea2" /></kbd>

Outcome of appyling Pauli Y to 0 and 1 state gives below -

<kbd><img width="117" height="60" alt="image" src="https://github.com/user-attachments/assets/14621012-7520-47ca-9815-f48d760167b8" /></kbd>
