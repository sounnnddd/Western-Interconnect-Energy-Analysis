# New York 2030 Business-As-Usual Power System Files

The following files contain power system data for New York state for the year 2030 following a buisness as usual policy.

	GenX Inputs
	  1. Capacity_reserve_margin
	  2. Energy_share_requirement
	  3. Fuels_data
    4. Generators_data
    5. Generators_variability
    6. Load_data
    7. Minimum_capacity_requirement
    8. Network
    9. Period_map (only TDR inputs)
    10. Representative_Period (only TDR inputs)
    Time Domain Reduction Runs
	Extra Outputs
		1. existing_gen_units
		2. site_cluster_assignments


### Capacity_reserve_margin
This file outlines regional capacity reserve margin requirements. Note that each region has a different reserve marginpercentage associated with it. 

### Energy_share_requirement
This file specifies regional policies for renewable portfolio standards and clean energy standards, mandating a minimum level of energy generation from qualifying resources. Qualifying technologies are specifed further in the Generators_data file

### Fuels_data
This file details fuel type, CO2 emissions intensity, and time-series data for fuel prices. Fuels are seperated by both technology type and region.

### Generators_data
This file details both existing and new build resources for the model, including cost and performance data as well as storage and demand flexibility resources. Additionally, tags are included on specific resources so that policies can be applied when solving.

### Generators_variability 
This file outlines the time-series data for capacity factor and resource availability. Note that every resource included in the Generators_data file is also included in this file.

### Load_data
This file provides time-series data for load profiles in each model zone, along with associated weights, load shedding costs, and optional time domain reduction parameters.

### Minimum_capacity_requirement
This file outlines the regional minimum requirements for technology capacity deployment.

### Network
This file defines the network topology and includes data on transmission fixed costs, capacity parameters, and loss parameters.

## Extra Outputs

### existing_gen_units
This file details all existing generator units for all IPM regions in the United States.

### site_cluster_assignments
These files help connect the clusters from the Generators_data file to real life sites. There is a file for every new renewable technology type for every region in the model. Further work would be needed to transform the GenX results into associated site data.

