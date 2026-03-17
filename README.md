# G4ILSCS

This repository contains the problem instances and the heuristic implementations used in the paper:

An integrated approach for lot-sizing and storage assignment

Repository Contents

- Problem instances used in the computational experiments:\
  NumT_NumI__Class1-3\
  NumT_NumI__Class4-6\
  NumT_NumI__Class7-9\
  NumT_NumI__big__Class10-14\
  Sensitivity Analysis_Handling-Costs\
  Sensitivity Analysis__Compatibility_90%\
  Sensitivity Analysis__Compatibility_80%\
  Sensitivity Analysis__Compatibility_70%\
  Sensitivity Analysis__Compatibility_60%\
  Note: see the file named 'NameClasses' inside the folders for more details about each class and data variation.

- Implementation of the heuristic solution approaches used in the paper:\
  RCLSP-MSL: Mathematical model solved by an Optimization package (Reformulated integrated capacitated multi-item lot-sizing and storage assignment problem with multiple capacitated storage locations)
  RFH: Benchmark Heuristic (relax-and-fix heuristic with time-oriented decomposition) \
  SH_v1: Sequential Heuristic - Version 1
  SH_v2: Sequential Heuristic - Version 2
  SH_v2_FO: Sequential Heuristic - Version 2 combined with Fix-and-Optimize Heuristic
  SH_v3: Sequential Heuristic - Version 3
  SH_v4: Sequential Heuristic - Version 4
  SH_v4_FO: Sequential Heuristic - Version 4 - combined with Fix-and-Optimize Heuristic

Paper Abstract:\
In this paper, we study the interaction between the lot-sizing problem and the storage assignment problem. Traditional lot-sizing problems have been studied for 
decades. However, only recent studies have further considered decisions related to the assignment of items to inventory locations, aiming to better model the
complex reality. In our problem, the storage space is divided into several separate locations, and the inventory is assigned to the storage locations taking 
into account specific compatibility conditions. Relocation of inventory is also possible if needed. In addition to the traditional cost elements from the 
lot-sizing problem, we consider others related to holding inventory, such as fixed storage costs, handling costs, and relocation costs. We model the problem 
using a general mathematical model, as well as a transportation reformulation, which provides better lower bounds. We propose several heuristics to solve the 
problem by splitting it into smaller subproblems, which are then solved sequentially. A series of computational experiments is carried out in order to evaluate 
the impact of the integration between the lot-sizing and the storage assignment decisions, as well as the behavior of the different solution approaches. The 
results show that the proposed heuristics are highly effective in finding feasible solutions that are very close to the best solutions, while spending 97%
less computational time compared to solving the full mathematical model. When compared to the relax-andfix heuristic (benchmark), certain versions of the 
heuristics can find better solutions using less computational effort, underscoring the benefit of employing more specialized heuristics. Additionally, we 
conduct a sensitivity analysis with the aim of understanding the impact of key input parameters on the problem. The results indicate a significant influence of 
compatibility levels on the problem complexity. Limited item–item compatibility notably increases complexity, whereas restricted item–location compatibility ]
reduces computational time.
