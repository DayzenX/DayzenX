import numpy as np
import matplotlib.pyplot as plt

# Define the quadratic equation
def quadratic(x):
    return x**2 - 4*x + 4

# Generate x values
x = np.linspace(0, 4, 100)

# Plot the quadratic equation
plt.plot(x, quadratic(x), label='y = x^2 - 4x + 4')

# Plot the roots
plt.scatter(2, 0, color='red', label='Root (2, 0)')

# Add labels and legend
plt.xlabel('x')
plt.ylabel('y')
plt.title('Graph of the Quadratic Equation')
plt.axhline(0, color='black',linewidth=0.5)
plt.axvline(0, color='black',linewidth=0.5)
plt.legend()

# Show plot
plt.grid(True)
plt.show()
