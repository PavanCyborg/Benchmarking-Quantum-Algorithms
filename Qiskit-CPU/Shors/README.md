This program performs Benchmarks of **Shor's** Algorithm on various simulators provided by **Aer** provider and also includes benchmarks performed with **FakeProviders**.



|Platform|Parameters|Noise Parameters|Benchmarks|Volumetric Positioning|Remarks|
|--------|----------|----------------|----------|----------------------|-------|
|qasm_simulator **method-1**(0.13.3)|min_qubits=10, max_qubits=30, max_circuits=2, num_shots=1000, basis: 1-['rx', 'ry', 'rz', 'cx']|***ideal***|![Test-1](1.jpg)|![Test-1-QV](1-QV.jpg)|Qasm simulator supports upto **31** qubits. Execution is terminated upto **30** qubits because of skip qubits parameter. |
|qasm_simulator (0.13.3)|min_qubits=3, max_qubits=12, skip_qubits=1, max_circuits=2, num_shots=1000,basis: 1-['rx', 'ry', 'rz', 'cx']|depol_one_qb_error = 0.05, depol_two_qb_error = 0.005, reset_to_zero_error = 0.005, reset_to_one_error = 0.005|![Test-2](2.jpg)|![Test-2-QV](2-QV.jpg)|Execution is terminated at **22** Qubits because of longer execution periods.|
|statevector_simulator (0.13.1)|min_qubits=3, max_qubits=13, skip_qubits=1, max_circuits=2, num_shots=1000,basis: 1-['rx', 'ry', 'rz', 'cx']|***ideal***|![Test-5](5.jpg)|![Test-5-QV](5-QV.jpg)|At 14 Qubits, Kernel is getting killed due to insufficient memory.|
|statevector_simulator (0.13.1)|min_qubits=3, max_qubits=14, skip_qubits=1, max_circuits=1, num_shots=1000,basis: 1-['rx', 'ry', 'rz', 'cx']|depol_one_qb_error = 0.05, depol_two_qb_error = 0.005, reset_to_zero_error = 0.005, reset_to_one_error = 0.005|![Test-6](6.jpg)|![Test-6-QV](6-QV.jpg)|Kernel getting killed at 13 Qubtis due to insufficent memory.|