# CI2024_lab2
Lab2 for Computational Intelligence Course at Polito

The approach for the TSP (Travel Salesman Problem) has been understood from the lectures. The road is in the following lines.
- The start is from an optimal solution for tsp, obtained with (1) or (2); where (1) is random and aproximate aproach, while (2) is obtained with a greedy algorithm proposed by the Professor.
- The solution is mutated N times, until is reached a number of individuals with a better fitness than the first solution. The mutation used is insert one, because the aim is to preserve the relative position of the elements.
- Then the parent selection is made with a tournament selection, so the champion of a group of individuals is picked.
- Between two parents the genetic operator is used, in particular crossover of type inver-over, that should preserve the relative order of genes (from one of the parents).
- This last two steps are continued until a steady-state is reached.   

The file "tsp-lab2.ipynb" lets the user choose between the different instances of the problem (executing only the part in which you are interested).

Some suggestions for the vector indexing operations were given by ChatGPT


Results obtained:

| Country   | Cost from Random Initialization  | Calls for random  | Cost from Greedy Initialization | Calls for Greedy |
|-----------|-------------|----------------------|-------------|-----------------------|
| Italy     | 16362       | 10201               | 4379        | 5000                 |
| US        | 621240      | 10229               | 47168       | 7955                 |
| China     | 974824      | 18150               | 62194       | 7880                 |
| Vanuatu   | 1396        | 10213               | 1345        | 5273                 |
| Russia    | 311005      | 10215               | 41944       | 6820                 |
