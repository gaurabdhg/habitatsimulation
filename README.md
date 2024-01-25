# Predator-Prey Model
The habitat is a 2D square, L = 10 units in size, periodic in all directions.
Each animal is represented by an agent. There are two types of agents: rabbits and wolves.
The simulations start with agents randomly distributed in the domain: Nr = 900 rabbits and Nw = 100 wolves.

Each rabbit behaves according to the following rules:
– Each time step it chooses random direction and makes a step of length sampled from the normal distribution with mean parameter µ = 0 and standard deviation parameter σ 
– Each time step it replicates with probability pr r = 0.02 (one more rabbit is created at the same position) 
– Each rabbit dies at the age of tr d time steps. At the simulation start, rabbits are created with the age (integer number) uniformly sampled from the interval [1,tr d).

Each wolf behaves according to the following rules:
– Each time step it chooses random direction and makes a step of length sampled from the normal distribution with mean parameter µ = 0 and standard deviation parameter σ 
– It eats a rabbit with probability pw e = 0.02 every time the rabbit gets within distance rc = 0.5 of the wolf (each time step the wolf can eat as many rabbits as there are in its vicinity) 
– It replicates with probability pw r = 0.02 every time it eats a rabbit (it can replicate multiple times during single time step if it eats multiple rabbits) 
– It dies from hunger if it does not eat for tw d = 50 time steps

The system is initialised with random distribution of rabbits and wolves in the domain. Step size parameter σ equal to 0.5 both for rabbits and wolves. Rabbits die at the age of tr d = 100 time steps. 

Simulations look at the evolution of the number of rabbits and wolves in time. 
####Possible extension: Consider the Lotka-Volterra equations (https://en.wikipedia.org/wiki/Lotka-Volterra equations). Our model does not exactly corresponds to these equations.

We try different parameters to study evolution in different conditions.
