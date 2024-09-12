# Traveling Salesman Problem (TSP) is NP-hard

## Theorem

The Traveling Salesman Problem (TSP) with a known starting and ending position, where both positions are different, is NP-hard.

### Proof

#### Reduction from Hamiltonian Cycle Problem (HCP)

##### HCP

* **Input**: Graph G = (V, E)
* **Question**: Does G have a Hamiltonian cycle?

##### TSP

* **Input**: Complete graph K_n, starting vertex s, ending vertex t, edge weights w(u, v)
* **Question**: Find the shortest tour that starts at s, ends at t, and visits each vertex exactly once

#### Reduction Steps

1. Construct K_n from G
2. Set s and t to distinct vertices
3. Set w(u, v) = 1 if (u, v) in E, 2 otherwise

#### Correctness

* If G has a Hamiltonian cycle, then K_n has a tour of length n
* If K_n has a tour of length n, then G has a Hamiltonian cycle

#### NP-hardness

* HCP is NP-complete
* TSP is NP-hard since we reduced HCP to TSP

[[Tags: NP-hardness, Traveling Salesman Problem, Hamiltonian Cycle Problem]]