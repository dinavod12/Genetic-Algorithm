# Genetic-Algorithm
Genetic Algorithm Optimization on CEC Benchmark Functions

This repository contains an implementation of a Genetic Algorithm (GA) applied to various CEC benchmark functions, including:

    Bent Cigar Function
    Rosenbrock Function
    Rastrigin Function
    Ackley Function
    Griewank Function
    Schwefel Function

The primary focus of this project is to explore the effects of varying mutation rates and crossover rates on the performance of the Genetic Algorithm in optimizing these benchmark functions.
Project Overview

Genetic Algorithms (GAs) are powerful optimization techniques inspired by the process of natural selection. They use populations of candidate solutions to iteratively improve upon solutions through the application of genetic operators, such as selection, crossover (recombination), and mutation.

In this project, we test different combinations of:

    Mutation rates: controlling how frequently the algorithm introduces random changes to individual solutions.
    Crossover rates: determining how often two parent solutions recombine to produce offspring.

By adjusting these parameters, we aim to study their influence on the convergence behavior and performance of the GA across different problem landscapes provided by the benchmark functions.
Benchmark Functions

The CEC benchmark functions used in this study are widely recognized in optimization research for their distinct characteristics and varying levels of difficulty:

    Bent Cigar Function: A unimodal function with a sharp contrast between one smooth direction and one sharp ridge.
    Rosenbrock Function: Known for its narrow valley with a global optimum, it poses challenges due to its slow convergence.
    Rastrigin Function: A highly multimodal function characterized by numerous local minima, making it difficult for algorithms to find the global optimum.
    Ackley Function: A multimodal function with a nearly flat outer region and a large hole at the center.
    Griewank Function: A function with many widespread local minima but only one global optimum.
    Schwefel Function: This deceptive function is known for its large search space and global optimum located far from most of the search points.

Implementation Details

    Initialization: Random initialization of the population with real-valued vectors.
    Selection: Roulette wheel selection or tournament selection can be used to choose parents for crossover.
    Crossover: Various crossover rates are tested, from low to high, to study their effect on the population's diversity and convergence.
    Mutation: Different mutation rates are explored to understand their role in escaping local minima and maintaining diversity.
    Evaluation: Each individual's fitness is calculated using the benchmark functions.
    Termination: The algorithm terminates either when a maximum number of generations is reached or when the population fitness converges.


Results and Analysis

The results section presents a comparative analysis of different mutation and crossover rates for each benchmark function. Plots and tables show the convergence behavior, highlighting how different parameter combinations influence the GA’s ability to find the global optimum.

This repository is intended for researchers, students, and developers interested in optimization algorithms, particularly Genetic Algorithms, and their application to complex optimization problems. Contributions and suggestions are welcome!
How to Use

    Clone the repository:

    bash

git clone https://github.com/dinavod12/genetic-algorithm-cec-benchmark.git

Install the required dependencies:

pip install -r requirements.txt

Run the optimization script with different parameter settings:

css

python run_ga.py --mutation_rate 0.01 --crossover_rate 0.7 --function bent_cigar
