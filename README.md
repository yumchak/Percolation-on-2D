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
