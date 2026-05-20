How to run the HSR Simulation Program



Open SIMEX.XLS, SIMEX1.XLS and SIMEX2.XLS in directory D:\HSR.  When the dialog box says “ This document contains links. Re-establish links?” Click on “NO”.

Select Worksheet ‘Data’ in SIMEX1.XLS

	Enter the Trainset Capacity (Cell R11C5).
	Enter the Period when there is a demand for transport (Cell R19C7).
	Enter the Fares for the different OD Markets (Cells R24C3:R28C3 and R24C6:R27C6).
	Enter the Supply Characteristic “TauxMax” (Cell R23C9) as defined in the “Supply 	Characteristics” Section.
	Enter the time between two Services (Cell R14C7) which is the amount of time a trainset must 	stay at the destination station before being available to head out once again for a new service.

Select Worksheet ‘Data (exp)’ in SIMEX1.XLS

	Enter the Northbound Travel Demand for the different OD Markets (Cells R7C6:R15C6).
	Enter Travel Time for Los Angeles-Bakersfield (Cell R29C4), Bakersfield-Fresno (Cell R30C4),
	Fresno-San Jose (Cell R31C4) and San Jose-San Francisco (Cell R32C4) Segments.
	Enter the Actual Stopping Time for Bakersfield (Cell R30C6), Fresno (Cell R31C6) and San Jose 	(Cell R32C6) Stations.
	Enter the Total Stopping Time for Bakersfield (Cell R30C8), Fresno (Cell R31C8) and San Jose 	(Cell R32C8) Stations.

Select Worksheet ‘Data (exp)’ in SIMEX1.XLS

	Enter the Commercial Capacity (Cell R4C14) as defined in the “Supply Characteristics” Section.
	Enter the Total Number of Service provided between Los Angeles and San Francisco per 	direction (Cell R2C12). It has been calculated in the report as the ratio between the total travel 	demand on the most heavily trafficked segment and the commercial capacity.
	Enter Delta (Cell R6C13) as defined in the “Step 1 : Service Attractiveness” Section
	Choose the number of Express Services and Non-Stop Services retained for the Simulation. 
	The method used in the report is to maximize the number of Non-Stop Services subject to the 	constraint that Ecart (Column 11) is positive.
	Copy the retained number of Express Services and Paste.Special (Value) in Worksheet ‘Data 	(exp)’ in SIMEX1.XLS in Cell R7C9. Copy the corresponding E[Exp] and Paste.Special (Value) 	in Cell R7C10.
	Copy the retained number of Non-Stop Services and Paste.Special (Value) in Worksheet ‘Data’ 	in SIMEX1.XLS in Cell R7C9. Copy the corresponding E[NS] and Paste.Special (Value) in Cell 	R7C10.
	

If the Travel Demand is not symmetric, activate SIMEX2.XLS and repeat the same operation.
Once new formula have been entered in SIMEX2.XLS worksheets ‘data’ and ‘data (exp)’ links between SIMEX2.XLS and SIMEX1.XLS do no longer exist. Thus, a genuine version of SIMEX2.XLS should be kept when running the simulation for non-symmetric travel demand.

Activate SIMEX.XLS.

	Click on     at the right upper corner of the screen.
	If the simulation is run on another computer, select worksheet ‘Simex’, select Cell R1C1 choose 	Macro in the Tools Menu and click on Run.


The HSR Simulation Outputs


Northbound   Open LA-SFO1.XLS and EXPRESS1.XLS in directory D:\HSR\LA-SFO.
	Worksheet ‘Bilan’ in LA-SFO1.XLS provides the Non-Stop Service Travel Demand Allocation 	as well as the Los Angeles-San Francisco Schedules.
	Worksheet ‘Resultats’ in LA-SFO1.XLS provides the Non-Stop Service Load Factors and 	Revenues.
	
	Worksheet ‘Demand’ in EXPRESS1.XLS provides the Express Service Travel Demand 	Allocation for every OD Markets served as well as the Load Factors for every Segment of the 	new line. ‘Demand’ also shows the early morning travel demand on Secondary Markets from 	Bakersfield and Fresno which is not served by Los Angeles-San Francisco Services. When the 	level of the demand is high enough, additional services originating in Bakersfield or Fresno or 	leaving Los Angeles before 5 A.M. can be run.
	Worksheet ‘Revenue’ in EXPRESS1.XLS provides the Express Service Revenues for every OD 	Markets served.
	
Southbound   Open SFO-LA1.XLS and EXPRESS2.XLS in directory D:\HSR\SFO-LA 
Fleet Movements and Number of Trainsets required  Open LA-SFO1.XLS in directory D:\HSR\LA-SFO. Worksheet ‘Trainset’ provides the fleet movements for trainsets based in San Francisco and Los Angeles as well as the number of trainsets required to provide services. This number is usually increased by 5% in order to take into account the non-disposability of a proportion of the total fleet due to defection or maintenance.
	
	Fleet movements can be simulated with different values for the minimal required time between 	two services as defined in SIMEX1.XLS Worksheet ‘Data’ Cell R14C7.
	Open RAME.XLS in directory D:\HSR. Select Worksheet ‘Ref’ and Cell R1C1. 
	Enter the new value.
	Click on     at the right upper corner of the screen.
	If the simulation is run on another computer, select worksheet ‘Rame’, select Cell R3C2 choose 	Macro in the Tools Menu and click on Run.

	
Prior to run a new simulation, output files must be moved from the D:\HSR\LA-SFO or the D:\HSR\SFO-LA directory. They may be renamed and moved in the D:\HSR\OUTPUT  directory.
