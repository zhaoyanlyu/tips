# Multivariate Gaussian
----
# PDF:

There are two forms of multivariate Gaussian distribution, one is for real number, one is complex number.

Real:

$$
P(\mathbf{x})=(2\pi)^{-\frac{d}{2}}\det(\Sigma)\exp
\Big(-\frac{1}{2}(\mathbf{x}-\mathbf{\mu})^\top\Sigma^{-1}(\mathbf{x}-\mathbf{\mu})\Big)
$$

Complex:

$$
P(\mathbf{x})=\pi^{-d}\det(\Sigma)\exp
\Big(-(\mathbf{x}-\mathbf{\mu})^\mathrm{H}\Sigma^{-1}(\mathbf{x}-\mathbf{\mu})\Big)
$$

where the $\mathbf{x}$ is a random vector follows multivariate Gaussian distribution $\mathbf{x}\sim\mathcal{N}(\mathbf{\mu}, \Sigma)$ with dimension of $d$. The $\mathbf{\mu}$ is the expectation vector and $\Sigma$ is the covariance matrix. $\top$ represent transpose and $\mathrm{H}$ is the conjugate transpose (also known as 'Hermitian transpose').
