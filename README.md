# CME212 Submission Repository

## Problem 1
This is your CME212 homework repository. Feel free to edit your README and any other files!

I added 4 cores in the setting in virtual box to allow the Virtual Linux System on my mac to run the mass_spring executable on potentially 4 cores. The following results are shown below in a table after running on different grid sizes for grid0, grid1, grid2, and grid3. 

Table of Results: Values are in **seconds**
 
|             Grid Size                          | thrust::system::omp::par | thrust::system::detail::sequential::seq |
|------------------------------------------------|--------------------------|-----------------------------------------|
| **grid0**										 | 148.637                  | 155.018                                 |
| **grid1**										 | 141.23                   | 178.846                                 |
| **grid2**										 | 292.818                  | 139.668                                 |
| **grid3**										 | 419.49                   | 322.858                                 |

The results shown in the tables are :
* Plane Constraint
* Applying Sphere Constraint 1, Move around Sphere
* Applying Sphere Constraint 2, Remove Nodes Within Sphere

It is clear from the table that for the smaller grid sizes the sequential procedure using thrust is faster however and thus the parallel method is at a disadvantage, as the grid size is refined the the parallel procedure from thrust starts to pick up and create an advantage as seen in grid sizes 2 and 3. 

## Problem 2




