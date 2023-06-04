# CAT-tickets
Analysis of CAT ServiceNow tickets

## Questions
+ what locations are the most active?
+ who are the most prolific callers?
+ what is average number of tickets each year per day/week?
	+ for each system
+ how long on average does it take for CAT to resolve the issue (before Jan 19, 2023 and after the revamp)?
+ what is average agent workload?
	+ each system must be treated separetly
	+ take into account # of agents at the time (before and after)
	+ any imbalances between agents' workloads

+ what are proprtions of ticket types?
+ how often tickets are miscategorized by callers?
+ how often tickets are not for CAT?
+ how often issue to resolve orginated in other dept. than CAT?
+ on average how many actions were needed to resolve the ticket?


## Exports from ServiceNow
Generate a list of tickets to be selected and export to csv format the following fields:
+ number
+ crated
+ caller
+ created_by
+ state (u_bkop_state)
+ category
+ subcategory
+ assigment_group
+ bpl_location
+ nypl_location
+ resolved
+ assigned_to
+ u_bpl_or_nypl
+ mat_source
+ close_code
+ url
+ reassignment_count
+ updates
+ sys_mod_count
+ resolved_by

Save .csv files in `\src_data` directory. This data in raw form should not be made public.

## Sampling guidelines
Some of the questions may require sampling and evaluation of tickets.

Consider:
+ how large the sample should be? consider manual review workload.
+ does it need to be proportional to popularity of the subcategories?
