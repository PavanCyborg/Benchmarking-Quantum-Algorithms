This program performs Benchmarks of **Hidden Shift** Algorithm on QSim's Density matrix simulator.


|Platform|Parameters|Noise Parameters|Benchmarks|Volumetric Positioning|Remarks|
|--------|----------|----------------|----------|----------------------|-------|
|dm_simulator|min_qubits=2, max_qubits=14, skip_qubits=2(default), max_circuits=2, num_shots=1000, basis: 1-['rx', 'ry', 'rz', 'cx']|***ideal***|![Test-1](1.jpg)|![Test-1-QV](1-QV.jpg)|dm_simulator supports upto 31 qubits. Execution is limited to **14** Qubits.|
|dm_simulator|min_qubits=2, max_qubits=14, skip_qubits=2(default), max_circuits=2, num_shots=1000, basis: 1-['rx', 'ry', 'rz', 'cx']|options_noisy = {"thermal_factor": 0.9,'show_partition': False,"decoherence_factor": 0.9,"depolarization_factor": 0.9,"bell_depolarization_factor": 1,"decay_factor": 0.75,"rotation_error": {'rx':[1.0, 0.0], 'ry':[1.0, 0.0], 'rz':[1.0, 0.0]},"tsp_model_error": [1.0, 0.0]}|![Test-2](2.jpg)|![Test-2-QV](2-QV.jpg)|Execution is limited to **14 Qubits** due to timing & memory constraints.|