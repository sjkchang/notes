## Actors
- Organization Functions
	- Testing 
		- Security Testing
		- Performance Testing
	- Audit
		- Security Audit
		- Compliance Audit
		- Process Audit
- Business Ops Leadership
	- Ops-Executive
	- Ops Mangers
	- Ops Superusers
- Engineering VP
	- Track 1
		- Engineering Director
			- Eng. Lead
			- Product Architect
			- Solution Architect
		- Vendor Team
			- Scrum Master
			- Product Owner
			- Solution Architect
			- Software Architect
			- Development Lead
				- Developer 1
				- ...
				- Developer n
			- Test Lead
				- Tester 1
				- ...
				- Tester n
- Program Managements
	- Program manager
	- Billing coordinator
	- Sales coordinator
	- Contracts coordinator
	- vendor leadership

## Inception
Define the vision and request the work

**_Steps_**
- Product owner speaks to stakeholder to develop High Level Requirements
- High Level Requirements are broken down into Epics
- Epics preview is shared with software Architect and Dev Leads

## Planning
_**Steps**_
- Product owner works with software architect to break epics into stories
- Acceptance criteria is added and priority is added
- Dependencies are highlighted
- Spring refinement takes place with wider audience
- Team questions clarifies and refines the stories
- Team weighs the stories with story points
- Backlog is marked refined
## Execution
**_Steps_**
- Team picks stories from the refined backlog based on priority and available capacity
- Team commits to delivering story points
- ScrumMaster starts the spring and monitors progress with daily standups
- Team keeps storyboard updated with remarks and current status
- If capacity remains they picak another item from the freined backlog
- End of the spring, ScrumMaster analyzes the completion of the committed work


**_Story Life Cycle_**
-  Pending ->
- In Progress -> 
- Review ->
- QA Development ->
- QA Ready ->
- QA Review ->
- PO Acceptance ->
- Done ->
- UAT Deployment ->
- QA + Business Ops Signoff ->
- Prod change request creation ->
- Review by change approval board ->
- Prod Deployment ->
- QA + Business Ops Signoff 

**_Site Reliability Engineering_**
-  Setup build pipelines using Kubernetes, Docker, Jenkins for each service/app
- Manage docker's base image
- setup vulnerability checks using fortify
- setup code scans using SonarQube
- Monitor production services
- Configure k8s config maps and secrets
- Renew Credentials & manage certificates
- Support UAT and PROD deployments

**_Deployments_**
- QA deployments are managed by developers and supported by SRE
- UAT and PROD deployments are done by STE post-QA and user signoffs are procured and all evidence is attached in the service now tickets



