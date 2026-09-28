# Dataset Description

This dataset provides a summary of the worker-weighted access by different census geography levels and travel times for the state. The worker-weighted access here represents the number of jobs a person can reach at 8am from a specific census area within a given travel time threshold. The travel time threshold are in integer minutes, at intervals from 5 minutes to 60 minutes (1 hour).

Census levels included in this dataset are:

	1. Block
	2. Block Group
	3. Census Tract
	4. County
	5. State

The data for each census level is presented as a separate CSV file.

## Data Files

{state_name}_{state_id}_{mode}_{summary_level}_{year}.csv: These files contains that state's census level data for that individual mode.  

### Important Note

Due to its large size, the 'Block' level data file should not be opened outside of a person's coding platform. Attempting to open this file in Excel or a similar spreadsheet program would cut off a significant amount of data.

## Data Fields

	1. Mode: the travel mode, one of auto; bike; transit; or walk
	2. Year: NAE data year
	3. State FIPS: the ID of the containing geography within which the data averages are calculated
	4. Summary Level: the level of geography at which averages are calculated; one of state, county, census tract, block group, or block
	5. Census ID: the ID of the particular census geography for which the data averages are calculated 
	6. Departure: the time of day a mode's accessibility is measured.
	7. LTS: Level of Traffic Stress, measured only for bike mode.
	8. Threshold: the travel time threshold in minutes, ranging from 5 to 60 minutes
	9. Weighted_average_total_jobs: the average number of jobs a person can reach from a given census area within the travel time threshold for a specific mode
