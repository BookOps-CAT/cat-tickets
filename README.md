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
+ sys_created_on
+ u_caller
+ sys_created_by
+ u_bkop_state
+ u_subcategory
+ u_bpl_or_nypl
+ u_bk_location
+ location
+ assigned_to
+ u_resolved
+ u_resolved_by
+ u_close_code
+ u_admin_url
+ sys_mod_count

## Sampling guidelines
Some of the questions may require sampling and evaluation of tickets.

Consider:
+ how large the sample should be? consider manual review workload.
+ does it need to be proportional to popularity of the subcategories?
