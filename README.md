# Solving the Number Partitioning Problem with Simulated Annealing and QAOA

## The Number Partitioning Problem

Number partitioning - also referred to as the number bi-partitioning problem, or the 2-partition problem - is one of Karp’s original NP-hard problems, and can be stated as follows. We have a set S of n numbers, and the goal of the optimisation problem is separate them into two disjoint subsets S1 and S2 such that the difference of the sums of the
two subsets is minimised. 

For example, if ```S = {4, 5, 6, 7, 8}```, then one possible partition would be ```S1 = {4, 8}``` and ```S2 = {5, 6, 7}```. The sums of
these two subsets are 12 and 18 respectively, giving a difference of 6. The optimal solution is ```S1 = {4, 5, 6}```, ```S2 = {7, 8}```,
since the sum of both of these subsets is 15, and hence the difference is zero.

## Code files
### Simulated Annealing (SA)
* [```number-partitioning-simulated-annealing.ipynb```](Simulated Annealing/number-partitioning-simulated-annealing.ipynb): Jupyter notebook containing the Julia implementation of SA
* ```number-partitioning-pyqubo.ipynb```: Jupyter notebook containing the Python implementation of SA using pyqubo and is useful for cross-checking solutions against the Julia version of SA
* ```writeup-sa-number-partitioning.pdf```: Write-up containing the pseudocode, approach and analysis of SA

### QAOA
* ```number-partitioning-qaoa.ipynb```: Jupyter notebook containing the QAOA class and the Qiskit Aqua implementation 
* ```number-partitioning-problem-set```: File containing values of the set to partition
* ```writeup-qaoa-number-partitioning.pdf```: Write-up containing the algorithm, approach and analysis of performance of QAOA with respect to the number of layers
