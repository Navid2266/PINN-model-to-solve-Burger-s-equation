# Burger's Equation Solved with Physics-Informed Neural Network (PINN)

In this repository, I implement a PINN (Physics-Informed Neural Network) to solve a simplified version of Burger's equation. The equation we aim to solve is:

∂U/∂t + U∂U/∂x = μ∂²U/∂x² 

For simplification, we have neglected the effect of viscosity (μ), setting it to 0 at first. The initial condition is defined as:

- **U(x, 0) = sin(πx)**, for x ∈ (0,1)

The boundary conditions are:

- **U(0, t) = 0**
- **U(1, t) = 0**

# About Physics-Informed Neural Networks (PINNs)

**Physics-Informed Neural Networks (PINNs)** are machine learning models designed to solve physics-based problems by incorporating known physical laws into the learning process. Unlike traditional neural networks that only rely on data, PINNs enforce physics equations as constraints during training, making them more accurate and interpretable.

PINNs combine data from experiments or simulations with physical principles, optimizing a loss function that balances data accuracy and adherence to the governing equations. This allows them to effectively solve complex, nonlinear problems in fields like fluid dynamics, heat transfer, and solid mechanics, even when data is limited or noisy.

Also For more on PINNs, you can check out these resources by Maziar Raissi:

- https://arxiv.org/abs/1711.10561
- https://arxiv.org/abs/1711.10566

# Results

As demonstrated in the provided image, the model accurately predicts the solution to the equation, with a mean squared error of only 0.05. The PINN effectively captures the dynamics of the system.


![image](https://github.com/user-attachments/assets/f06a0117-8bff-4fcf-a3c9-7b09102c962f)
