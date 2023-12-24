# Genetic-Algorithm-for-Finding-Optimal-Solutions
Simulate genetic selection to find optimal parameters.
import random

def fitness_function(solution):
    # Example fitness function
    return sum(solution)

def genetic_algorithm(population_size, generations):
    population = [[random.randint(0, 1) for _ in range(5)] for _ in range(population_size)]
    for generation in range(generations):
        population = sorted(population, key=fitness_function, reverse=True)
        # Perform crossover and mutation operations
        # Update the population based on fitness
    return population[0]

optimal_solution = genetic_algorithm(100, 50)
print("Optimal Solution:", optimal_solution)
