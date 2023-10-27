Types of attack on 3 tier architecture  [[Final]]
- Web Browser
	- Man in the Middle
	- Cookie Stealing
	- 
- Sever
	- XSS - Cross Site Scripting
	- DDOS - Distributed Denial of service
- Business Logic
- Database
	- SQL Injection

### Threat Modeling
Analyze what can go wrong in your distributed architecture

Pragmatic (good) vs Pessimistic (bad)
_Key Questions_
- What are you building?
- What can go wrong?
- What should you do about what can go wrong?
- Did you do a good job of analysis?

Attack Vector 


Attack Pattern

Attack Actions
- Probe - Try ports until a vulnerable port is found
- Scan - Try specific port to see if it is exposed
- Flood - Large volume of unauthorized requests to stress load
- Authentication
- Bypass
- Spoof
- Read
- Copy
- Steal
- Modify
- Delete


#### Trust Boundaries
- Web browser - | Web server - Business Logic | - | Database |

#### Attack Surface
The Attack Surface of an application is:
1. the sum of all paths for data/commands into and out of the application, and
2. the code that protects these paths (including resource connection and authentication,
authorization, activity logging, data validation and encoding), and
3. all valuable data used in the application, including secrets and keys, intellectual property,
critical business data, personal data and PII, and
4. the code that protects these data (including encryption and checksums, access auditing,
and data integrity and operational security controls).

#### Trust Boundaries Vs Attack Surface

### Federated API
Expose one central API server to consumer. When consumer wants a specific api service, the request is made to the central API server which then directs the message to the specific service.
This decreases the number of attack surfaces as the central api server and specific api services are in the same trust boundary.

_Examples_
- APIM 
- Apogee


### STRIDE
Process to determine what could go wrong with distribued system. It is a mnemonic for things that can go wrong in security

- **S**poofing - Pretending to be something or someone you are not
- **T**ampering - Modifying something you are note supposed to modify. Ex: Packet on wire, bits on disk or bits in memory
- **R**epudiation - Claiming you didn't do something regardless of whether or not you did it
- **D**enial of Service - Attack designed to prevent a system from providing its services, by crashing it, making it unusably slow, or filling all of it's storage
- **I**nformation Disclosure - exposing information to people who are unauthorized to see it
- **E**levation of Privileges - when a program or user is technically able to do things that they are not supposed to do.

### DREAD
Methodology for risk rating vulnerabilities. Threat risk 0-10
- Damage Potential
- Reproducibility
- Exploitability
- Affected Users
- Discoverability

### Common Attack Pattern Enumeration and Classification (CAPEC)
List of all well known vulnerable attack patterns that have no software solution 
