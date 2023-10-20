### 25 Years Ago

#### Monolith Development Lifecycle
	- Large monolith app (5 GB C Binary)
	- Weekly Release cycle (ideally, but not in practice)
	- Lots of inter-team gating due to monolith

### Breaking the Monolith
- Broke into [[Microservice]] architecture 
- AWS Amazon Web Services developed from this change
	- Amazon recognized breaking into small web services solved some of there issues maybe other people would want it
- [[DevOps]]: Is integrated with each team
	- Team responsible for developing a service must also develop the DevOps monitoring systems
	- Two Pizza Teams
		- Someone always on-call to help fix customer problems
		- Must respond, whatever the time
	- Decentralized
	- Agile
	- Autonomy
	- Accountability
	- Ownership

Self Service Tool Example: Apollo

### Pipelines 
- [[Continuous delivery]]
- Automated release process
- Faster more reliable release
- Adopted by virtually all teams

Amazon used **_Pessimistic Deployments_**
- No guarantee that in a real life scenario everything will be successful
- Solution
	- On new release direct some traffic to on box.
	- If traffic is normal and not having issues/ meets requirements
		- Deploy to one availability zone (physically separated/geographically distanced deployment zones)
		- If service is behaving normal, expand to more availability zones
			- Deploy to one more region
				- Same Process until confident that it can be fully rolled out
	- Fully automated system

Optimized Edit-Compile-Test ECT Loop
- Must get a code review to move on to next phase of deployment
- Uses AI tools to help autocomplete code and fix common errors (Similar to Copilot)
	- Trained on Own Codebase so internal libraries are recommended
		- 27% Growth in productivity when it was added
- ECT is best place to catch errors.

Want to catch problems/errors as early as possible
ECT -> Code Review -> Staging -> Productions

#### Monitor and Measure Everything
Ops Culture
- How to ensure quality across thousands of teams
	- Amazon prioritizes customer satisfaction

Weekly Ops Meeting

Listen to Customers
- Working Backwards
	- Every new service must have a press release and FAQ, before you build the product
	- Forces consideration of how customers will view the service
	- Brainstorming with customers before development even begins
	- 

- Resource Monitoring
	- CPU, Memory, ect
- Application monitoring
- Canary monitoring
- Client-side monitoring
- Order drop rate monitoring
	- Even if everything works if people are dropping services, something is wrong