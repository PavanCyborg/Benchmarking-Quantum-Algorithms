This program performs Benchmarks of **Grover's Search** Algorithm on QSim's Density matrix simulator.


|Platform|Parameters|Noise Parameters|Benchmarks|Volumetric Positioning|Remarks|
|--------|----------|----------------|----------|----------------------|-------|
|dm_simulator|min_qubits=2, max_qubits=10, skip_qubits=1, max_circuits=2, num_shots=1000, basis: 1-['rx', 'ry', 'rz', 'cx']|***ideal***|***TBD***|***TBD***|dm_simulator supports upto 31 qubits.|
|dm_simulator|min_qubits=2, max_qubits=10, skip_qubits=1, max_circuits=2, num_shots=1000,basis: 1-['rx', 'ry', 'rz', 'cx']|options_noisy = {"thermal_factor": 0.9,'show_partition': False,"decoherence_factor": 0.9,"depolarization_factor": 0.9,"bell_depolarization_factor": 1,"decay_factor": 0.75,"rotation_error": {'rx':[1.0, 0.0], 'ry':[1.0, 0.0], 'rz':[1.0, 0.0]},"tsp_model_error": [1.0, 0.0]}|![Test-2](2.jpg)|![Test-2-QV](2-QV.jpg)|Execution is limited to **10 Qubits** due to timing constraints.|