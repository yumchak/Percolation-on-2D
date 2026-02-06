## BACKGROUND

**Percolation theory** describes the connectivity of a randomly structured network or lattice. The mathematical study of percolation has been widely applied in fields such as materials science, epidemiology, earth science.
In real life, it is often used to describe the flow of liquid through in soil or the process of coffee brewing. 

In this project, our investigation focuses on the percolation in 2-dimensional grids, studying its connectivity and understanding its behaviour in random lattices. 
We build a percolation model in an $n \times n$ square grid. Each site of the $n \times n$ square grid is coloured yellow (occupied/ open) with probability $p$, and blue (closed) with probability $1−p$. Two sites are considered adjacent if their coordinates differ by 1 either vertically or horizontally. We assume each site of the grid is independent, which means whether one site is open or closed, does not influence the state of any other site in the grid.

In this percolation model, it is only possible to connect through adjacent and open sites. We aim to study the probability $F_n(p)$ that there is a yellow path connecting the left boundary to the right boundary of the grid.

$ F_n(p) = \mathbb{P}(\text{there is a yellow path connecting left to right on an } n \times n \text{ grid}). $
, which 
$\lim_{n \to \infty} F_n(p) = F(p),$
This represents the probability of an open path connecting the left and right boundaries. Moreover, we investigate different situations and extensions of the model.

By running simulations with different grid sizes $n$ and open grid probability $p$, we can estimate the critical probability $p_c$. When a critical percolation occurs, i.e. $p$ is around $p_c$, $F_n(p)$ shows sharp transition. This sudden change in behaviour is called **"phase transition"**

----
### This project is divided into six sections, which focus on:
1. **Grid Visualisation** $n \times n$ grid in different p values.

2. **Building Algorithm** 
- Function to determine the connectivity of random grids 

- Optimising the estimation of the function for larger n.

3. **Estimate Critical probability p_c** by simulations 

4. **Explore Variations** Percolation behavior in different geometry 
- Percolation on Rectangular grid. 

- Centre to boundary connectivity. 

5. **Percolation on Triangular lattice** 
- Percolation on Triangular lattice. 

- Asymptotic power law behaviour near $p_c$ for triangular lattice. 

- Crossing probability of Triangular lattice after roatation. 


6. **Alternate detect methods**

- Wall-following algorithm and site exploration behaviour.

- Uniform Random Labels & Minimum Threshold Estimation. 

  
Throughout this project, we use Python as our programming language, also utilised NumPy and Matplotlib to help generate grids and simulations. We conduct topic research, observate model behavior, analyse data and explore the emergence of connectivity.

------
## Contribution
This project was completed as part of a group assignment. I was responsible for
the implementation and analysis in **Section 3** and **Section 5**, including
the percolation simulation, BFS/DFS connectivity checks, and the corresponding
Monte Carlo experiments.




## Background

**Percolation theory** studies the connectivity of randomly structured networks
or lattices. It has wide applications in materials science, epidemiology, and
earth science. In real life, percolation is often used to describe phenomena
such as the flow of liquid through soil or the process of coffee brewing.

In this project, we investigate percolation on two-dimensional grids, focusing
on connectivity and probabilistic behaviour in random lattices. We construct an
$n \times n$ square grid, where each site is independently coloured yellow
(open) with probability $p$ and blue (closed) with probability $1 - p$. Two sites
are considered adjacent if their coordinates differ by 1 vertically or
horizontally.

Connectivity is only possible through adjacent open sites. We study the
probability $F_n(p)$ that there exists a yellow path connecting the left boundary
to the right boundary of the grid:
\[
F_n(p) = \mathbb{P}(\text{there exists an open path connecting left to right on an } n \times n \text{ grid}).
\]

As $n \to \infty$, $F_n(p)$ converges to a limiting function $F(p)$. By running
Monte Carlo simulations for different grid sizes $n$ and occupation
probabilities $p$, we estimate the critical probability $p_c$. Around $p_c$,
$F_n(p)$ exhibits a sharp transition, a phenomenon known as a **phase
transition**.

---

### Project Structure

This project is divided into six main sections:

1. **Grid Visualisation**  
   Visualising $n \times n$ grids for different values of $p$.

2. **Algorithm Construction**  
   - Connectivity detection on random grids  
   - Optimisation for large $n$

3. **Critical Probability Estimation**  
   - Estimation of $p_c$ using Monte Carlo simulation

4. **Model Variations**  
   - Percolation on rectangular grids  
   - Centre-to-boundary connectivity

5. **Percolation on the Triangular Lattice**  
   - Triangular lattice percolation  
   - Asymptotic power-law behaviour near $p_c$  
   - Crossing probabilities under lattice rotation

6. **Alternative Detection Methods**  
   - Wall-following algorithms  
   - Uniform random labels and minimum threshold estimation

Throughout the project, Python is used as the primary programming language, with
NumPy and Matplotlib for simulation and visualisation. The project combines
algorithm design, simulation, and data analysis to study the emergence of
connectivity in stochastic systems.

---

## Contribution

This project was completed as part of a group assignment. I was responsible for
the implementation and analysis in **Section 3** and **Section 5**, including the
percolation simulation, BFS/DFS connectivity checks, and the corresponding Monte
Carlo experiments.

