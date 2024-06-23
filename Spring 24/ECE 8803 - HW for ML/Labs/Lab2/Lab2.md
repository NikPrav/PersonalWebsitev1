- Launch scalesim through `$ python3 scale.py -c <path_to_config_file> -t <path_to_topology_file> -p <path_to_output_log_dir>`

# Requirements
- Config file, with the arch spec
	- arch spec for this lab
- Topology file, with the workload topology
	- topology for this lab
Do a design space exploration through running the sim multiple times, and get mapping efficiency

# Tasks
- 2 A.1 - DSE
	- A.1 ii) 
		- total number of cycles < 10000
		- mapping efficiency > 90
		- get ==system.cfg== and ==COMPUTE_REPORT.csv==
	- A.1 iii)
		- total number cycles < 17500
		- area < 15000
		- get ==system.cfg== and ==COMPUTE_REPORT.csv==
		- 3 plots - 
			- Total cycles vs MAC units with SRAM = 1kb, 3 graphs for each dataflow
			- Total cycles vs MAC units with SRAM = 2kb, 3 graphs for each dataflow
			- Total cycles vs MAC units with SRAM = 3kb, 3 graphs for each dataflow
- 2 A.2 - Faulty Systolic Array - ==4+1==
	- how do you calculate compute cycles with all the -1s
	- how to get number of tiles with all the -1s
	- how to create ifmap_demand_matrix. Is the ifmap_demand_matrix important?
		- get number of tiles
		- using number of tiles, replicate said array n times
		- said array will always have a length of M+2 per tile
- 2 B.1 - DSE with bandwidth - 
	1) DSE for bandwidth efficiency - ==1==
		- system.cfg and COMPUTE_REPORT.csv for 94 percent ME
	2) Run DSE for given values of L1 and L2 - ==2==
		- Report with plot
			- x-axis Ifmap L1/(L1 + L2)
			- y-axis average bandwidth/ stall cycles
			- different graphs for different Filter L1/(L1 + l2) - done
	- Run DSE for different ratios of double buffering - ==2==
		- same two graphs
	- one para about role of stuff
- 2 B.2 - Compute cycles for different dataflows - ==5== - done
	- modify dataflow.py 
	- assume different dataflows and calculate expected compute cycles
		- weight stationary
		- input stationary
		- output stationary
		- row stationary