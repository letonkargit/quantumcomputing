<Details>
  <summary>Qiskit Library Installation</summary>
        
        pip install qiskit
        
        pip install qiskit-ibm-runtime
        
        pip install 'qiskit[visualization]'
        
        import numpy as np
</Details>

## Hadamard Operator
Define
      
      H = Operator([[1/np.sqrt(2), 1/np.sqrt(2)],[1/np.sqrt(2), -1/np.sqrt(2)]])
      
Matrix representation

      H.draw("latex")
      
<kbd><img width="104" height="67" alt="image" src="https://github.com/user-attachments/assets/2582efd7-1a38-43b7-9e2e-56bc67f5e0b0"/></kbd>

## Hadamard on QuantumCircuit
Define Quantum Ciruit
      
      hdemo = QuantumRegister(1, "Q1")
      qc = QuantumCircuit(hdemo)
      qc.draw("mpl")
<kbd><img width="147" height="109" alt="image" src="https://github.com/user-attachments/assets/effe3843-18b4-4a7b-b1b5-6e9b3bd7dd07" style="border:1px" /></kbd>

Look at state

    Statevector.from_circuit(qc).draw("latex")

<kbd><img width="63" height="40" alt="image" src="https://github.com/user-attachments/assets/c674d704-5520-442a-ad06-ea315fbbfc1b" /></kbd>

Apply Hadamard on Qubit 1

    qc.h(hdemo)

<kbd><img width="178" height="108" alt="image" src="https://github.com/user-attachments/assets/80f6d82c-442d-4122-a31c-b85c085fde20" /></kbd>

State after Hadamard is applied

<kbd><img width="128" height="67" alt="image" src="https://github.com/user-attachments/assets/4e443ae1-8a1c-47c3-a4b3-00b2c1216c21" /></kbd>

This is nothing but a |+> (called ket plus)<br>
Below are the outcomes for the input qubits(copied from IBM site)<br>

<kbd><img width="236" height="62" alt="image" src="https://github.com/user-attachments/assets/9f3031c0-2219-4317-b5f3-f5927641f05b" /></kbd>
