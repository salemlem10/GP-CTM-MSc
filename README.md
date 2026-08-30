# GP-CTM-MSc
# GP-CTM: Goal Programming Cell Transmission Model

Multi-objective traffic demand management model from my MSc thesis at Kansas State University. Extends Ziliaskopoulos's cell transmission network LP formulation with a goal programming structure, so demand release and congestion are traded off explicitly rather than optimized as a single objective.

**Network:** Sabah Al Salem Block 1, Kuwait — 120 cells, 6 sources, 5 sinks, 60-minute horizon at 10-second timesteps, 7,000 vehicles of demand.

**Goals:** total admitted demand, total network occupancy, and sink throughput, each with a target and a deviation variable. The objective minimizes the weighted sum of deviations.

**Result:**  all three goals met. ~115 seconds in Gurobi.

**To run:** open `GP-CTM.ipynb` and run all cells. Requires gurobipy, pandas, numpy, matplotlib, and a Gurobi license.

Presented at the IISE 2026 Annual Conference (full proceedings publication).
