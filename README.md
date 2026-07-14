# Quick Start

1) Download the docker-compose.yml and create a new folder for the docker image
Note: it is recommended to run create a directory outside of your Desktop folder (or any folder that is cloud sync'd in Windows or Mac)

2) Ensure Docker Desktop is installed and running, then run the command:
$docker compose pull

3) Ensure it successfully pulls the package and then start it up by running the command:
$docker compose run --rm sl2cfoam /bin/bash

4) Once inside the container navigate to something interesting such as:
root@145030b1288d:/workspace/sl2cfoam-next-master/faocc_or_weighted/faocc_or_weighted_v7#
root@145030b1288d:/workspace/sl2cfoam-next-master/faocc_or_weighted/faocc_or_weighted_v8/preflight# 

5) The README_v7_structured.md has a comprehensive set of tests that yielded the results in preparation for the next tests descibred at the end of the summary below.

- Finite-Aeon OR-Combinatorial Cosmology: https://doi.org/10.13140/RG.2.2.24944.11524/6
- FAOCC-LQG: A Fixed-Graph Twistor and Spinor Bridge to OR-Selected Quantum-Geometric Histories: https://doi.org/10.13140/RG.2.2.21714.31683

# From Spin-Foam Amplitudes to a Recoupling-Covariant Pre-OR Operator in FAOCC–LQG

Finite-Aeon OR-Combinatorial Cosmology (FAOCC) proposes that the physically realized histories of a cosmological aeon form a finite subset of the much larger space of formal quantum possibilities, with objective reduction supplying the physical distinction between unrealized alternatives and realized branch events. To investigate how such a selection principle might be incorporated into loop quantum gravity without altering standard kinematics, this program develops and tests a fixed-graph numerical framework based on Lorentzian EPRL spin-foam vertex amplitudes. Full five-index vertex tensors were generated with `sl2cfoam-next` and deformed only after the ordinary EPRL calculation by applying a bounded, dimensionless geometry-aligned weighting to their intertwiner components. The weighting used recoupling-angle and shape-regularity information as a preparatory proxy, while deliberately avoiding any claim that it represented a Penrose–Diósi gravitational self-energy or a microscopic collapse law. Its effect was measured through component-basis participation and, more importantly, through one-axis and (2|3) bipartite singular-value spectra, which provide more stable measures of how quantum-amplitude support is distributed across the tensor.

The resulting support concentration survived an extensive hierarchy of controls. It was directional under reversal of the proxy, stable under rank normalization and equivalent amplitude- versus probability-level implementations, and reproducible across canonical relabelings, numerical environments, and booster cutoffs from dℓ=5 to dℓ=12. In ensemble tests involving ten B1 representatives, five C1 response-class representatives, three deformation strengths, and 10,000 random proxy permutations per representative, all 90 primary singular-spectrum tests remained significant after multiple-testing correction. The effect also remained exceptional after normalizing compression by Jensen–Shannon deformation of the underlying probability distribution. These results show that the proxy is not merely imposing generic sparsity: its alignment with the EPRL amplitude structure produces a statistically specific redistribution of support. At the same time, the component-basis results were less universal, reinforcing the conclusion that singular-spectrum measures (not raw basis sparsity) are the appropriate diagnostics.

A subsequent SU(2) recoupling audit exposed the central mathematical limitation and its resolution. Explicit Clebsch–Gordan and Wigner-(6j) maps transported undeformed EPRL tensors with near-unit fidelity and satisfied orthogonality, unitarity, and composition tests at approximately machine precision. Transporting one fixed weighting operator between recoupling frames largely removed the apparent orbit dependence, whereas independently rebuilding a diagonal proxy in every frame produced several inequivalent operators. The scalar proxy therefore did not define a unique physical observable. A complete canonical-orbit average was then constructed by transporting all B1 operators into a common basis and averaging them over the permutation orbit. The resulting operator is unique within the tested sector, non-diagonal, recoupling-covariant, monotonically compressive, and robust under removal of any individual source representative. In a stronger null test using 10,000 randomized covariant operator averages, none matched the real operator’s one-axis or (2|3) compression, either at orbit level or across the ten target representations. 

So far, the outcome has provided a concrete pre-OR operator architecture for FAOCC–LQG: standard EPRL amplitudes remain intact, while an additional covariant operator selects a more concentrated subset of quantum-geometric support. The construction does not yet establish objective collapse. The next step is to determine whether independently defined angle, volume, shape, Regge-curvature, quasilocal-energy, or matter-density operators can explain the successful empirical operator and be promoted to a two-history, energy-valued functional capable of supporting a physical collapse timescale and stochastic branch-selection dynamics.


<img width="1448" height="1086" alt="EPRL Spin-foam L2" src="https://github.com/user-attachments/assets/25ffea90-038f-4740-adf9-9f85823d8f11" />

<img width="1536" height="1024" alt="5 Tetra" src="https://github.com/user-attachments/assets/51f84e69-420a-4194-902e-3d89f0184944" />

<img width="1536" height="1024" alt="D2_Permutation" src="https://github.com/user-attachments/assets/b1f4caf5-a304-47cf-a24b-f7211d540999" />

<img width="1149" height="1369" alt="EPRL_120orbit_OR" src="https://github.com/user-attachments/assets/4bd808e3-72a1-401e-bdc7-fe9f15af9209" />

<img width="1149" height="1369" alt="ERPL_OR_view" src="https://github.com/user-attachments/assets/3dfde428-4ee2-46c0-9464-c03557e0a1fc" />

# Acknowledgements
- This project builds upon and utilizes the following open-source works:
Francesco Gozzini, A high-performance code for EPRL spin foam amplitudes, Class. Quantum Grav. 38, 225010, https://doi.org/10.1088/1361-6382/ac2b0b
- Repo: https://github.com/qg-cpt-marseille/sl2cfoam-next

