This program performs Benchmarks of **Grover's Search** Algorithm on Braket's simulators.


|Platform|Parameters|Noise Parameters|Benchmarks|Volumetric Positioning|Remarks|
|--------|----------|----------------|----------|----------------------|-------|
|LocalSimulator(Statevector)|min_qubits=3, max_qubits=14, skip_qubits=1, max_circuits=3, num_shots=1000|***ideal***|![Test-1](1.jpg)|![Test-1-QV](1-QV.jpg)|Execution terminated after **14** Qubits due to lack of memory.|
|LocalSimulator(dm_simulator)|min_qubits=3, max_qubits=11, skip_qubits=1, max_circuits=3, num_shots=1000|***ideal***|![Test-2](2.jpg)|![Test-2-QV](2-QV.jpg)|after **11** Qubits, it is taking long time to execute.|
|LocalSimulator(dm_simulator)|min_qubits=3, max_qubits=11, skip_qubits=1, max_circuits=3, num_shots=1000|noises.BitFlip(probability=0.01), noises.PhaseFlip(probability=0.1), noises.Depolarizing(probability=0.1), noises.TwoQubitDepolarizing(probability=0.1), noises.TwoQubitDephasing(probability=0.1), noises.AmplitudeDamping(gamma=0.1),noises.GeneralizedAmplitudeDamping(gamma=0.1, probability=0.1), noises.PhaseDamping(gamma=0.1), noises.PauliChannel(probX=0.1, probY=0.2, probZ=0.3)|![Test-3](3.jpg)|![Test-3-QV](3-QV.jpg)|after **11** Qubits, it is taking long time to execute.|
