# Wireless Network Deployment Optimization

This repository contains a project on planning optimization for wireless network deployment. The goal of the project is to design a cost-efficient wireless infrastructure for a telecom operator while guaranteeing coverage and performance requirements over a target area. The deployment problem considers candidate installation sites and two possible base station types: macro base stations, which provide larger coverage at higher cost, and micro base stations, which are cheaper but have shorter range. The project investigates whether it is more effective to deploy only macro stations, only micro stations, or a combination of both.

The problem is formulated as a Mixed-Integer Linear Programming (MILP) model. The optimization minimizes the total installation cost of deployed base stations while ensuring that each test point is assigned to exactly one active base station, that the received power satisfies a minimum receiver sensitivity threshold, and that the achievable peak throughput is at least 7 Mbps. The throughput is computed using Shannon’s formula, based on received power, noise, and bandwidth. This mathematical formulation makes it possible to compare deployment strategies under realistic engineering constraints.

Three main deployment scenarios are evaluated in the project. The first scenario considers only macro base stations, the second considers only micro base stations, and the third allows a mixed deployment of both types. The results show that macro-only deployment requires fewer stations but leads to the highest overall cost. Micro-only deployment is significantly cheaper, although it requires a larger number of stations due to the smaller coverage radius of micro cells. The mixed deployment achieves the best cost-performance tradeoff by combining the advantages of both options.

According to the results, the macro-only scenario has a total cost of 7.99 with 4 macro base stations, while the micro-only scenario has a total cost of 4.77 with 12 micro base stations. The best solution is obtained with the mixed deployment, which uses 1 macro base station and 9 micro base stations for a total cost of 4.58. This represents a cost reduction of about 42.7% compared with the macro-only scenario and about 3.9% compared with the micro-only scenario. The mixed strategy therefore provides the most efficient deployment in terms of both cost and number of installed stations.

The project also includes a sensitivity analysis to study the effect of stricter receiver sensitivity thresholds and higher throughput requirements. The results show that when the receiver sensitivity becomes more demanding or when the minimum throughput increases, the required number of base stations and the total deployment cost rise across all scenarios. Even under these variations, mixed deployment consistently provides the best or near-best balance between network performance and deployment cost.

Overall, this project demonstrates how optimization techniques can be applied to wireless network planning in order to support engineering decisions in telecommunications. It combines mathematical modeling, radio coverage analysis, throughput constraints, and scenario comparison in a practical deployment framework.

## Authors

Zahra Nazar Zadeh Attar and Yalda Mirzaee
