# **GPU and CPU Particle Swarm Optimization (PSO) Repository**

This repository implements a parallelized Particle Swarm Optimization (PSO) algorithm in both CPU and GPU versions, designed for optimizing a variety of benchmark objective functions. The repository demonstrates the speed advantages of GPU computation by leveraging **CuPy** for GPU-based calculations, as well as the traditional **NumPy** library for CPU-based calculations.

### **Key Features:**
1. **Benchmark Objective Functions**:
   - Implementations of popular optimization functions such as **Sphere**, **Rosenbrock**, **Rastrigin**, **Ackley**, **Schwefel**, **Griewank**, **Levy**, and **Michalewicz** for testing and optimizing.
   - Functions are optimized for both CPU and GPU environments, ensuring compatibility with a wide range of hardware setups.

2. **Particle Swarm Optimization (PSO)**:
   - **CPU Implementation**: A standard PSO implementation using **NumPy** for sequential computation, ideal for smaller optimization problems or environments without GPU access.
   - **GPU Implementation**: A fully vectorized PSO implementation using **CuPy**, which allows for massively parallel processing on compatible GPUs, significantly accelerating optimization for large search spaces or high-dimensional problems.

3. **Performance Comparison**:
   - The repository includes a benchmark comparing the CPU and GPU versions of PSO. Performance is evaluated based on runtime, demonstrating a **speedup of up to 30x** when using GPU acceleration.
   - Results for **optimal positions**, **fitness values**, and **execution times** are provided to showcase the efficiency gains of GPU-based optimization.

4. **Customizability**:
   - Supports custom bounds and parameter configurations, such as swarm size, inertia weight (ω), and acceleration coefficients (cognitive and social components).
   - Flexible API for integration into custom optimization workflows, with easy-to-use function wrappers for different objective functions.

5. **Scalability**:
   - The GPU implementation efficiently handles large swarms and high-dimensional problems, making it suitable for use cases in areas like machine learning, data science, engineering, and financial optimization.

### **Usage**:
- Simply modify the bounds and swarm size to suit the problem at hand.
- Choose between the CPU or GPU versions based on your hardware and performance requirements.
- Benchmark performance with the provided objective functions or add custom functions as needed.

### **Benefits**:
- **Accelerated Computation**: The GPU-based version provides substantial performance improvements, especially for large and complex optimization problems.
- **Ease of Use**: Simple function calls allow users to quickly integrate PSO into their optimization tasks, with minimal setup required.
- **Versatility**: Supports a wide range of problems from standard benchmark functions to custom real-world optimization tasks.

This repository is ideal for anyone looking to perform high-dimensional optimization using PSO, with the added benefit of GPU acceleration for faster results.
