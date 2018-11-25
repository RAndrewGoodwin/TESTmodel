Test model
Version 2019 R1

Tool for testing hypothetical behavior rules to see what the outcomes (trajectory and distribution) are when played together with grid-based data, for example:
 - water hydraulic patterns
 - water quality or contaminants
 - remotely sensed terrestrial landscapes
 - air/wind flow patterns
for situations where the environment could be responsible for individual animal, robot, cell, swarm, or other agent movement of interest.

This tool allows such investigation using large 2D, 3D, and time varying grids storing the environmental data.

Instructions for getting started are located in the folder "Install_and_GettingStarted", which includes some hints for programming newcomers just interested in using the ELAM model.

Behavior rules are located entirely within "BehaviorRule.f90" in the "ELAMsourceCode/solver" folder. Code files supporting "BehaviorRule.f90" are located in the "ELAMsourceCode/solver" folder. The Fortran coding language is used for the behavior rules and supporting material because of debate that Fortran may be easier than C++ for beginners to use; Fortran is also fast. Fortran code may be converted to C++ depending on future preferences of users.

C++ code (.cpp and .h files) link the ELAM model behavior rules and supporting computations with the Tecplot commercial library, so one can use a simple laptop to run the ELAM model on large grids, e.g., grids with many millions of nodes, including the generalized case of moving 3D grids of n-faced polyhedra used in some environmental modeling applications.
