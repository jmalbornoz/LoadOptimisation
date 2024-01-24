# LoadOptimisation
An example of how to use contraint optimisation to produce a load plan for a small fleet of vehicles.

The purpose of packing problems is to determine the optimum way to pack a collection of items with varying sizes into containers with defined capacities. A typical application is efficiently putting boxes onto delivery vehicles. Due to capacity limits, it is frequently impossible to pack all of the products. In that case, the problem is to determine a subset of the items with the most significant overall size that will fit in the containers.

There are many types of packing problems. Knapsack problems and bin packing are two of the most common.

**Knapsack problem**

The knapsack problem is a combinatorial optimization problem in which you must decide how many items should be included in a container. The overall weight of the collection must be less than or equal to a specific limit. The problem derives its name from the dilemma faced by someone who is constrained by a fixed-size knapsack and must fill it with the most valuable items.

The issue frequently arises in resource allocation when decision-makers must choose among various non-divisible projects or tasks under a defined budget or time limit.

**Bin packing problem**

Similar to the knapsack problem, the bin packing issue is also an optimization problem. A finite number of bins or containers, each with a defined capacity, must be packed to minimize the total number of bins used.

Filling containers, loading vehicles with weight capacity limits, making file backups in media, technology mapping in FPGA semiconductor chip design, putting boxes onto delivery vehicles are all examples of the problem.

**The problem at hand**

We need to load a number of items with certain weights and volumes onto a number of vehicles, each with a given maximum volume and weight capacity. The loading must be done in the most efficient way so that the unused capacity for each vehicle is minimised.

We will show how this problem can be solved using [Google's OR-Tools library](https://developers.google.com/optimization). 
OR-Tools is open source software for combinatorial optimization, able to find the best solution to a problem out of an extensive set of possible solutions. Here are some examples of problems that OR-Tools addresses:

* Vehicle routing: Find optimal routes for vehicle fleets that pick up and deliver packages given constraints.
* Scheduling: Find the optimal schedule for a complex set of tasks that need to be performed before others on a fixed set of machines or other resources.
* Bin packing: Pack as many objects of various sizes as possible into a fixed number of bins with maximum capacities.

Problems like these typically have many viable solutions — too numerous for a computer to sort through. OR-Tools overcomes this by narrowing the search set with cutting-edge algorithms to obtain an optimal (or near-optimal) answer.
