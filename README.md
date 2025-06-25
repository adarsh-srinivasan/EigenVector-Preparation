# EigenVector-Preparation

In this repository, we implement the eigenvector preparation problem for diagonal unitary matrices. 

The goal of this project is to write a python function with the following inputs and outputs:

#### Input: 
A quantum circuit containing a diagonal unitary operator $U$, such that $U \Ket{x}_n = e^{2\pi\Theta(x)}\Ket{x}_n$, such that all values of $e^{2\pi\Theta(x)}$ are distinct, a number $d$, such that $2^d \Theta(x) \in \mathbb{Z}$ for each $x$, and a value $t \in [0,1]$ with the promise that there exists only one $x$ such that $e^{2 \pi i t}=e^{2 \pi i \Theta(x)}$. 

#### Output: 
Output $x$. 

The main function is grover(d,n, diag_entries), which takes as input numbers $d,n$ and an array of such diagonal entries, and outputs a quantum circuit that solves the problem described above. We can benchmark and test this code by running the notebook and change the parameters of the final cell. 
