This program performs Benchmarks of **VQE** Algorithm on various simulators provided by **Aer** provider and also includes benchmarks performed with **FakeProviders**.



|Platform|Parameters|Noise Parameters|Benchmarks|Volumetric Positioning|Remarks|
|--------|----------|----------------|----------|----------------------|-------|
|qasm_simulator |min_qubits=4, max_qubits=12, skip_qubits=2, max_circuits=2, num_shots=4092, basis: 1-['rx', 'ry', 'rz', 'cx']|***ideal***|![Test-1](1.jpg)|![Test-1-QV](1-QV.jpg)|Reference files are only upto **12** Qubits.|
|qasm_simulator |min_qubits=4, max_qubits=12, skip_qubits=2, max_circuits=2, num_shots=4092, basis: 1-['rx', 'ry', 'rz', 'cx']|depol_one_qb_error = 0.05, depol_two_qb_error = 0.005, reset_to_zero_error = 0.005, reset_to_one_error = 0.005|![Test-2](2.jpg)|![Test-2-QV](2-QV.jpg)|Reference files are only upto **12** Qubits.|
|statevector_simulator |min_qubits=4, max_qubits=12, skip_qubits=2, max_circuits=2, num_shots=4092,basis: 1-['rx', 'ry', 'rz', 'cx']|***ideal***|![Test-3](3.jpg)|![Test-3-QV](3-QV.jpg)||
|statevector_simulator |min_qubits=4, max_qubits=12, skip_qubits=2, max_circuits=2, num_shots=4092,basis: 1-['rx', 'ry', 'rz', 'cx']|depol_one_qb_error = 0.05, depol_two_qb_error = 0.005, reset_to_zero_error = 0.005, reset_to_one_error = 0.005|![Test-4](4.jpg)|![Test-4-QV](4-QV.jpg)||
|FakeAlmaden (1.4.6)|min_qubits=4, max_qubits=12, skip_qubits=2, max_circuits=2, num_shots=4092,basis: 1-['rx', 'ry', 'rz', 'cx']|***Provider's Preset***|![Test-5](5.jpg)|![Test-5-QV](5-QV.jpg)||
|FakeAlmadenV2 (1.4.6)|min_qubits=4, max_qubits=12, skip_qubits=2, max_circuits=2, num_shots=4092,basis: 1-['rx', 'ry', 'rz', 'cx']|***Provider's Preset***|![Test-6](6.jpg)|![Test-6-QV](6-QV.jpg)||