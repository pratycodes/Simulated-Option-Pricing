# Monte Carlo Simulation-Based Derivatives Pricing Library

This project implements a Monte Carlo simulation-based engine for pricing vanilla and exotic options using the Geometric Brownian Motion (GBM) model. The library is designed for educational purposes and showcases the implementation of parallelization with OpenMP to speed up Monte Carlo simulations.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Dependencies](#dependencies)
- [Installation](#installation)
- [Usage](#usage)
- [Running Tests](#running-tests)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This C++ project implements a Monte Carlo-based engine for pricing financial derivatives, specifically European and Asian options, using the Geometric Brownian Motion (GBM) model. The project incorporates parallelization using OpenMP to speed up Monte Carlo simulations, improving performance when simulating large numbers of paths.

The library can be used to price:
- European Call/Put options
- Arithmetic Asian Call/Put options

## Features

- **Monte Carlo Simulation**: Pricing of European and Asian options using Monte Carlo methods.
- **Geometric Brownian Motion (GBM)**: Utilizes the GBM model to simulate the underlying asset price.
- **Parallelization with OpenMP**: Uses OpenMP to parallelize Monte Carlo simulations, speeding up the process.
- **Modular Design**: The code is modular and allows for easy extension to include more complex option pricing methods.

## Dependencies

- **C++17**: The code is written in C++17.
- **OpenMP**: For parallelizing the Monte Carlo simulations.
- **CMake**: To manage the build process.

## Installation

### Prerequisites

Ensure you have the following tools installed:
- **C++ Compiler** (e.g., GCC or Clang)
- **CMake** (Version 3.10 or above)
- **OpenMP** (Can be installed via Homebrew on macOS: `brew install libomp`)

### Building the Project

1. Clone the repository:

   ```bash
   git clone https://github.com/pratycodes/Simulated-Option-Pricing.git
   cd MonteCarloLibrary
   ```

2. Create a `build` directory:

   ```bash
   mkdir build
   cd build
   ```

3. Run `cmake` to configure the project:

   ```bash
   cmake ..
   ```

4. Build the project using `make`:

   ```bash
   make
   ```

### Running the Tests

After building the project, you can run the tests (e.g., for European or Asian options pricing):

```bash
./TestOptionPricing
```

This will execute the Monte Carlo simulation for pricing European options and output the results.


## Contributing

Contributions are welcome! Feel free to fork the repository, make changes, and submit pull requests. Please make sure to adhere to the following guidelines:

- Write clear, descriptive commit messages.
- Ensure all tests pass before submitting a pull request.
- Follow the project's coding style and conventions.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
