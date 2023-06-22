# CAT-tickets
Analysis of CAT ServiceNow tickets

Jan 19, 2023 - CAT ServiceNow revamp

## Questions
+ what locations are the most active? (completed)
+ who are the most prolific callers? (completed)
+ what is average number of tickets each year per day/week? (completed)
	+ for each system (completed)
+ how long on average does it take for CAT to resolve the issue (before Jan 19, 2023 and after the revamp)? (completed)
+ what is average agent workload? (copmleted)
	+ each system must be treated separetly
	+ take into account # of agents at the time (before and after)
	+ any imbalances between agents' workloads

+ what are proprtions of ticket types? (completed)
+ what are average resolution times before and after reorganization? (completed)
+ how often tickets are miscategorized by callers? (sample analysis needed)
+ how often tickets are not for CAT? (sample analysis needed)
+ how often issue to resolve orginated in other dept. than CAT? (sample analysis needed)
+ on average how many actions were needed to resolve the ticket?
+ what ticket subcategories are obsolete and could be deleted?
	+ consider few last years


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
If possible merge with archived, historical data starting in 2013.

## Sampling guidelines
Some of the questions may require sampling and evaluation of tickets.

Consider:
+ how large the sample should be? consider manual review workload.
	+ use [sample size calculator](https://www.calculator.net/sample-size-calculator.html)
	+ last year data (do we need more?)
+ does it need to be proportional to popularity of the subcategories?
+ consider sampling RL "Other" ticket category. Why so large?
+ investigate how ODC affects number of tickets through a sample (consider for the next analysis?)
+ samples:
	+ RL Other category
	+ Circ item problems: item not linked, item record problem, item attached to wrong bib, location code error
		+ who's fault (origin)
		+ any patterns that could be used for training?
	+ Circ bib problems: call number error, call number question, call number missing, sierra bib record error, duplicate records, other(?)
		+ who's fault: vendor, in-house staff, in-house bots
		+ any patterns that should be address through training? Will requried detailed tags.
	+ examine nature of the Circ "Call number questions" tickets
	+ examine electronic resource tickets
		+ what vendor (Ovedrive, Naxos, etc.)
		+ nature of the problems
		


