##Entities
**Developer**: Has the ability to submit a softare package and receive license and vulnerability information from that software package or other software packages in the License and Vulnerability database. 

**Manager**: Has the ability to create and update policies from the policy database as well as retrieve a policy from the database by giving the policy name. 

##Processes
**Orchestrator**: Pushes the software package and software name to the License Scanner and the NIST Vulnerability Database as well as returns the License Results to the Developer. This process also pushes the License and Vulnerability results to the License and Vulnerability database. 

**License Scanner**: Takes in Software package and analyzes the software for potential licenses and returns those licenses to the orchestrator. 

**Request License and Vulnerability info**: Takes a Software name from the developer or the manager and returns license and vulnerability results from the License and Vulnerability database baseed upon the software name. 

**Retrieve Policy Info**: Takes a policy name from the manager and retrieves a policy based upon that name from the policy database and then returns that information back to the manager.  

**Edit Policy**: Takes policy updates and pushes that information to the Policy databse and returns the policy info to the manager. 

**Create Policy**: Takes a new policy from the manager and submits that policy to the policy database. 

##Data Flows


