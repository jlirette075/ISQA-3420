##Entities
**Developer**: Has the ability to submit a software package and receive license and vulnerability information from that software package or other software packages in the License and Vulnerability DB. 

**Manager**: Has the ability to create and update policies from the policy DB as well as retrieve a policy from the DB by giving the policy name. 

##Processes
**Orchestrator**: Pushes the software package and software name to the License Scanner and the NIST Vulnerability DB as well as returns the License Results to the Developer. This process also pushes the License and Vulnerability results to the License and Vulnerability DB. 

**License Scanner**: Takes in Software package and analyzes the software for potential licenses and returns those licenses to the orchestrator. 

**Request License and Vulnerability info**: Takes a Software name from the developer or the manager and requests license and vulnerability results from the License and Vulnerability DB based upon the software name. 

**Retrieve Policy Info**: Takes a policy name from the manager and retrieves a policy based upon that name from the Policy DB and then returns that information back to the manager.  

**Edit Policy**: Takes policy updates and pushes that information to the Policy DB and returns the policy info to the manager. 

**Create Policy**: Takes a new policy from the manager and submits that policy to the policy DB. 

##Data Flows
**Software Package**: Contains the software package to be scanned by the license scanner and NIST Vulnerability DB. 

**License Results**: Contains the results from the License Scanner and are being sent back to the developer and to the License and Vulnerability DB. 

**Vulnerability Results**: Contains the Vulnerablity results from the NIST Vulnerablity DB and are being sent to the License and Vulnerablity DB. 

**Software Name**: Contains the software name from either the developer or manager and gets sent to License and vulnerability DB. 

**L / V Results**: Contains the license and vulnerability results obtained from the License and Vulnerability DB and are sent back to the manager and/or the developer. 

**New Policy**: Contains the new policy that is being sent to the Policy DB. 

**Policy Name**: Contains the name of a policy to be sent to the retrieve policy info process and then to the Policy DB. 

**Policy Info**: Contains the information about the policy that was either requested or recently updated and is ultimately sent back to the manager. 

**Policy Updates**: Contains the updated policy from the manager that goes to the Edit Policy process and then sent to the Policy DB. 

##Data Stores
**NIST Vulnerability DB**: This is the database that holds all of the Vulnerability information about different pieces of software being queried by the Developer through the orchestrator. 

**License and Vulnerability DB**:  This is the database that holds all of the license and vulnerability information from obtained from the License Scanner and/or the NIST Vulnerability DB. 

**Policy DB**: This is the database that contains all of the policy information either being updated, created, or queried by the manager. 
