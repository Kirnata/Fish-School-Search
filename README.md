# Fish-School-Search 🐟
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)<br>
### The fish swarm algorithm (FSA) is a population-based/swarm intelligent evolutionary computation technique that was inspired by the natural schooling behavior of fish. FSA presents a strong ability to avoid local minimums in order to achieve global optimization.

## About algorithm
A school of fish is an aggregation of fish that move with approximately the same speed and orientation, maintaining a constant distance between them.In the FSS algorithm (J.B.M. Philo and F. Neto, 2008), fish swim in an aquarium, which is the domain of acceptable solutions in the search for food (the solution to the optimization problem), with the position of fish in it reflecting the current solution vector. Each n-dimensional fish location represents a possible solution to the optimization problem.
### The main stages
1. Population initialization<br>
* Random selection of the agent's position within the aquarium. <br>
* The algorithm limits the maximum allowed weight of agents. <br>
* All agents are assigned a value equal to half of the maximum weight.<br>
2. Migration of agents to the food source<br>
The number of iterations (iter) is used as the stopping criterion.
At each iteration of the cycle all agents overcome several stages:
* Individual stage of floating agents <br> 
* Instinctive-collective stage <br>
* Collective-volitional stage of swimming <br> 
### Test function
In addition, there is a test function EggHolder function (function(x)) and a function for sorting individuals by values of the function sort(x, f).
<img src="https://github.com/Kirnata/Fish-School-Search/raw/main/images/formula.png" width="700">

<img src="https://github.com/Kirnata/Fish-School-Search/raw/main/images/Eggholder.png" width="700">

## How to use?

**The input of FSS and FSS_mod is 7 parameters:**<br> 
**X_min** - vector of lower bounds of the search;<br> 
**X_max** - vector of upper bounds of search;<br> 
**N_agent** - number of fish in a school;<br> 
**iter** - number of iterations;<br> 
**Wmax** - maximum weight of fish;<br> 
**StepMax** - maximum (initial) step size;<br> 
**StepMin** - minimum (final) step size.<br> 

You can change the parameters of the function call at the end of the code file, e.g.:<br> 
`x = FSS_MOD([-512, -512, -512, -512], [512, 512, 512, 512], 1000, 1000, 50, 50, 10)`<br> 
Then:<br> 
`run ffs.py` 
or
`run ffs_mod.py`<br> 
