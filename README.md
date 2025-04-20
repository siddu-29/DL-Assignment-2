# DL-Assignment-2
1. Translation
Model Configuration.Input Embedding Size (m): 256.Hidden State Size (k): 256 (for both encoder and decoder).Sequence Length (T): 20 (fixed for both input and output).Vocabulary Size (V): 60.Architecture: Single-layer LSTM encoder and decoder.Decoding Strategy: Greedy decoding
Computation Complexity
The total number of computations performed by the network is calculated using the formula:
T × [8k(m + k) + kV]
Substituting the values:
20 × [8 × 256 × (256 + 256) + 256 × 60]
= 20 × [8 × 256 × 512 + 15360]
= 20 × [1048576 + 15360]
= 20 × 1063936
= 21,278,720
Total Computations ≈ 21.28 million operations
Parameter Count
The total number of parameters in the model is calculated using the formula:
2Vm + 8k(m + k + 1) + kV + V
Substituting the values:
2 × 60 × 256 + 8 × 256 × (256 + 256 + 1) + 256 × 60 + 60
= 30720 + 8 × 256 × 513 + 15360 + 60
= 30720 + 1050624 + 15360 + 60
= 1,100,464
Total Parameters ≈ 1.10 million
