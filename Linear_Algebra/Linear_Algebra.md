# Linear Algebra

> A good understanding of linear algebra is essential for understanding and working with many machine learning algorithms, especially deep learning algorithsms.


## Scalars, Vectors, matrices and Tensors
* **Scalars**: just a single number
* **Vectors**: an array of numbers
* **Matrices**: a 2-D array of numbers
* **Tensor**: 

## Multiplying Matrices and Vectors
* $A$ must have the same number of columns as $B$ has rows.
* $A$ is of shape $m*n$ and $B$ is of shape $n*p$ then $C$ is of shape $m*p$
$$C = AB$$
$$C_i,_j=\sum\limits_kA_i,_kB_k,_j$$
* **Dot product** between two vectors $x$ and $y$ of same dimensionality is the matrix product $x^Ty$
* computing $C_i,_j$ as the dot product between row $i$ of $A$ and column $j$ of $B$
### Matrix product operations
* **Matrix multiplication**
$$A(B+C) = AB + AC$$
$$A(BC) = (AB)C$$

## Identity and Inverse Matrices
* **Identity Matrix** ($I_3$)
$$\begin{bmatrix}1&0&0\\0&1&0\\0&0&1\\ \end{bmatrix}$$

* **Matrix Inverse**: $A$ inveres matrix is denoted as $A^{-1}$
$$A^{-1}A=I_n$$

* Invertibility
    * Matrix can't be inverted if..
        * More rows than columns
        * More columns than rows
        * Redundant rows / columns ("linearly dependent", "low rank")

## Linear Dependence and Span
* A linear system of equations can have:
    * No solution
    * Many solutions
    * Exactly one solution: this means multiplication by the matrix is an invertible function  

* **linear combination**
* **linear dependence**
* **linear independence**
* **span**
## Norms
* Functions that measure how "large" a vector is
* **$L^p$** norm
$$||x||_p = (\sum\limits_i|x_i|^p)^\frac{1}{p}$$
* **Euclidean norm**: usually use L2 norm, p=2 
* Max norm, infinite p: $||x||_\infin = \max\limits_i|x_i|$
* A norm is any function $f$ that satisfies the following properties:
    * $f(x) = 0 \Rightarrow (x=0)$
    * $f(x+y) \leq f(x) + f(y) \,\,$ (the **triangle inequality**)
    * $\forall\alpha \in R, f(\alpha x) = |\alpha|f(x)$

## SpecialKinds of matrices and Vectors
* **Unit vector**
$$||x||_2 = 1$$
* **Symmetric Matrix**
$$A = A^T$$
* **Orthogonal matrix**
$$A^TA = AA^T = I$$
$$A^{-1} = A^T$$

## Eigendecomposition
* Eigenvector and eigen value
$$A\upsilon = \lambda\upsilon$$
* Eigendecomposition of a diagonalizable matrix
$$A=Vdiag(\lambda)V^{-1}$$
* Every real symmetric matrix hs a real, orthogonal eigendecomposition:
$$A = Q\Lambda Q^{-1}$$

## Singular Value Decomposition
* Similar to eigendecomposition
* More genera; matrix need not be square
$$A = UDV^T$$

## The Moore-Penrose Pseudoinverse

## The Trace Operator

## The Determinant

