Verification - Are we building the product correctly?
Validation - Are we building the correct product?

## Verification
Evaluation of work products during a work phase
To determine if the product is built according to reqs and specs

- **Evaluate:** Plans, Requirement Specs, design specs, Code, Test cases
- **Using:** Tests, tests, tests, but also reviews and walk throughs
## Validation
Evaluating a software product during or at the end of development to see if it meets BR (business requirements)
 - Does it match the user's needs?
 - Does it fulfil it's intended use?
 Early validation
 - **Evaluates**: Specifications
 - **Using**: Reviews, scenarios, questionnaires, MVP with user feedback...
 Final/work product validation
 - **Evaluates**: software product/version
 - **Using**: Testing (e.g ACs)
## V-Model
![[Pasted image 20240311141417.png]]
- Waterfall-type development lifecycle
- Used in a lot of diff engineering
- Not popular with agile experts
- But shows V&V well


## Dealing with bugs
- Write/track bug reports
- Objective of a bug report:
	- Check if a similar bug has been reported already. If so check if it is the same, either lump it in or or reference if slightly diff
	- Make it as simple as possible to re-produce
	- explain how to reproduce 
	- Provide minimalistic source code and data
	- Provide meaningful details 
## Hypothesis Testing
- Model + Conjecture:
	- Logging in is a difficult thing to achieve well
	- I have a feeling there is a flaw with logging in - I don't think I even need to register to be able to log in
- Hypothesis:
	- That the logging in utility is compromised
- Possible testing methods:
	- Using the "back button" after logging out
	- Refreshing the page
	- Seeing if passwords are sent in plain tedxt
	- Logging in with admin/ unsecure log ins
	- Run SQL injections
 