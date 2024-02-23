# 2D Particle Filter Accelerator for Mobile Robot Indoor Localization and Pose Estimation
Particle filtering is a reliable Monte Carlo algorithm for estimating the state of a system in modeling non-linear, non-gaussian elements for estimation and tracking applications in various fields, including robotics, navigation, and computer vision. However, particle filtering can be computationally expensive, particularly in high-dimensional state spaces, and can be a bottleneck for real-time applications due to high memory consumption. This paper proposes a particle filter accelerator that employs a cellular automata-based pseudo-random number generator and an improved systematic resampler based on the Vose Alias method. The particles are distributed across several sub-filters, performing concurrent resampling and importance weights computations. The proposed accelerator leveraged the inherent parallelism and pipelining stages of FPGAs to perform the resampling stage in a parallel fashion, significantly enhancing the particle convergence time. The proposed accelerator deployed on the Zedboard (ZC7020) system-on-chip achieves a low execution time of approximately 4.63 μs, 21.3 % speedup, and 3.1 % area reduction compared to the recent particle filter accelerator. The proposed design also demonstrates modularity, achieved through multiple parallel hardware subfilters that provide high throughput for real-time sensor data processing. Furthermore, the proposed accelerator performs a high sampling frequency of 216kHz, making it suitable for high throughput and real-time applications.
The paper has been published in IEEE Access.
**https://ieeexplore.ieee.org/document/10418505**

