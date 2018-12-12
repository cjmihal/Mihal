The Diffusion Equation in 2-D (Cartesian)

The code is simple to use. Users input values where prompted; the code automatically checks the validity of input values for cell size, number of cells, etc.

The code solves for the 2-D Diffusion Equation in slab geometry by applying the Thomas Algorithm. Each cell is assigned within a matrix and the algorithm solves
at each point and compiles the answer. The code's outputs include the solution array, a 3-D plot of the solution, and uses Python's built-in linear algebra solver
to check the answer.

Code is operational and compiles, but currently runs incorrectly. I believe there is an issue with the array when I translated it from 1-D to 2-D,
but have been unable to identify the issue. Python's linear algebra solver is unable to solve as well, so clearly there is an issue with how I set up the array.

The code attempts to model in 2 dimensions (x and y) the diffusion of neutrons throughout the system given a linear source centered within the cells. The top and right
boundaries are vacuums - that is, neutrons that pass through the boundaries disappear from the system - while the bottom and left boundaries are reflective - neutrons
"bounce back" into the system.

I have also attached a working 1-D version of the code so users can see what to expect for a proper solution. The 1-D includes absolute error compared to
solving it deterministically.

The neutron source is restricted to the center of the given problem geometry in the current code. Also, it assumes homogeneity in the cells at this time;
it cannot currently account for different materials within the system and how neutron diffusion would differ.