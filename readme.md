# [Interference Assessment] Breakthrough in Radar Interference Assessment! Multi-relational Structure Entropy Technology Achieves Real-Time Precision "Diagnosis" [Attached MATLAB Code]

[Interference Assessment]Breaking Through the Difficulty of Radar Interference Assessment! Multi-relational Structure Entropy Technology Achieves Real-Time Precision "Diagnosis" [Attached MATLAB Code] Original EW Frontier, September 18, 2025, 19:22, Liaoning
The "pain points" of traditional evaluation indicators. Traditional evaluation indicators are mainly divided into two categories, but both have limitations:
•  
Signal layer statistical indicators: Measurement of noise suppression intensity is facilitated by Shannon entropy, Renyi entropy, or J/S ratio. However, these indicators are nearly insensitive to "forward-backward" type deception jamming and cannot effectively assess the impact caused by such interference.
•  
Innovative Solution: An Evaluation Framework Based on Multi-Relational Structure Entropy for Radar Interference Effects
1. Measurement - Map: Building a three-layer heterogeneous graph to transform the radar measurement error model into a three-layer heterogeneous graph (spatial, kinematics, signal), and all kernel width parameters are directly derived from hardware calibration and associated thresholds, ensuring the practicality and accuracy of the model.
•  
During a single scanning cycle, the radar's measurement of the i-th target within the airspace can be represented as, where is the measurement vector containing azimuth angle, range, radial velocity, and signal characteristics.
•  
After CFAR detection, all measurements exceeding the threshold are considered as nodes in the graph.
2. Multi-relational Edge Weight Construction: Define three relational layers on the basis of a node set, namely spatial, kinematics, and signal characteristics. The edge weights are defined using normalized Gaussian kernel functions to measure the similarity of traces across different dimensions.
•  
Space Relationship (** ****)**: Measuring the proximity of traces in physical space, the edge weight formula is as follows: where Δd is the distance difference, Δφ is the azimuth angle difference, and converts the angle difference into a distance unit.
•  
Kinematics relationship (** ****)**: Measuring the consistency of point traces in velocity space, where the edge weight formula is given by , and .
•  
Signal Characteristic Relation (** ****)**: Measuring the similarity of point traces to radar echo characteristics, the edge weight formula is.
3. Interference - Graph structure mapping: introduces an interference modulation coefficient to quantify the impact of interference. Modulate the ideal side-weight. This modeling can be used to analyze the impact of different interferences on each relationship layer. Form an adjacent tensor for subsequent entropy calculation. The modulation effects of different interferences are as follows:
Interference type
Mode of action
Impact on the Relationship Layer
Noise suppression
Generates noise that drowns out the real signal.
Signal characteristic layer similarity sharply decreases ( )
Latency - forwarding spoofing
Copy and delay forwarding target signals
Signal similarity is maintained at a high level (...), and the spatial and kinematic layer edge weights exhibit exponential decline with delay.
Cluster - bridging deception
DRFM synergistically generates intrinsically related pseudo-clusters
Enhanced cross-cluster connectivity between intra-cluster nodes; inter-cluster nodes; bridging nodes
4. Multi-relational stochastic walks and structural entropy: Definition of evaluation metrics, define multi-relational Markov chains. The steady-state distribution of the transfer matrix is solved by power iteration. Subsequently, the entropy of a first-order multirelational structure is defined. And adopts the two-dimensional minimum MrSE () as the final evaluation index. Remove the clusterable structural information from the figure. Measure the level of "uncompressible" chaos in a scenario.
•  
First-order multirelational structure entropy formula:
•  
2D Minimum Entropy Formula:
5. Traditional Indicators "Frame-Incorporation": Realizing Comparative Analysis To enable traditional indicators to be comparable with MrSE at the same temporal and spatial resolution, the false alarm rate (FAR) and track continuity (TC) are "frame-incorporated".
•  
Frame-wise false alarm rate: the proportion of false points within all points in the current scan.
•  
Intra-frame trajectory continuity: C is the number of connected components formed by a subset of real target nodes, and N_T is the number of real target nodes.
Experimental Verification: Outstanding Performance and Stability
1. Experimental Design: The Monte Carlo simulation was used to design four interference scenarios (no interference, noise suppression, shadow deception, and noise + deception composite), each scenario being run independently for 2000 simulations. Simultaneously, a sensitivity analysis was conducted on three kernel width parameters, allowing them to vary independently from the baseline value, resulting in 27 parameter combinations, with each combination running 500 rounds of four-scene simulations.
2. Overall Discriminative Ability: As interference evolved from no interference (S0) to composite interference (S3), the median and overall distribution of the two-dimensional minimum MrSE (MRSE) showed a strict stepwise monotonic increase. From an initial 12.29±0.89 bits at S0, it significantly climbed to 19.17±2.26 bits at S3, with a one-way ANOVA showing significant differences among the four groups (p<0.001), effectively distinguishing between scene complexity differences caused by different interference patterns.
3. Strong Correlation with Traditional Indicators
MRSE is strongly positively correlated with frame-level false alarm rate (FAR), with a correlation coefficient (95% BCa CI: [0.719, 0.739]), and a p-value far less than 0.001.
MRSE is also moderately negatively correlated with frame-level track continuity (TC), with a correlation coefficient (95% BCa CI: [-0.475, -0.440]), and a p-value far less than 0.001. This indicates that the "structural disorder" measured by MRSE is highly coupled with the degradation of radar system performance (increased false alarms and track breaks). It can serve as an effective proxy indicator for assessing interference effectiveness.
4. Robustness of parameters is excellent. A ±30% perturbation analysis was conducted on three core kernel width parameters. Under 27 parameter combinations, the mean correlation coefficient between MrSE and FAR was 0.800 with a standard deviation of only 0.020, ranging from [0.754, 0.849]. Moreover, when parameters are perturbed, MrSE's ability to distinguish among four interference strategies remains significant, allowing for stable and reliable evaluation results without the need for fine-tuning parameters.
Engineering value and future prospects: MrSE can be integrated into the existing radar signal processing chain as an "in-built diagnostic" tool, aiding in dynamic power allocation and anti-jamming scheduling. It offers "unified, interpretable" advantages, eliminating the need for experience-based tuning, facilitating practical deployment applications.
Future directions include:
• Conduct field verification to further test the performance of this evaluation framework in real environments.
•
Expand it to multi-radar network scenarios to enhance the assessment capability of radar jamming effects in complex combat environments.
•
Construct an adaptive anti-jamming closed-loop based on MrSE gradients to achieve smarter and more efficient radar jamming scheduling.
The radar jamming effect evaluation framework based on multi-relational structure entropy breaks through the limitations of traditional metrics, providing a novel and efficient solution for radar jamming assessment. It holds significant application value and broad development prospects in the modern electronic warfare field.
End

## Images

![(Interference Assessment)Breakthrough in radar interference assessment! Multi-relational structure entropy technology achieves real-time and precise "diagnosis" [Attached MATLAB code]](cover.jpg)

<!-- PAYMENT_BLOCK -->

## Get this dataset

- Payment link (Stripe): [Buy now](https://buy.stripe.com/3cs8yP7sY87d0vu9AB)
- Payment QR code: ![Payment QR code](pay.png)

<!-- /PAYMENT_BLOCK -->
