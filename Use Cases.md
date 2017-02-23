##Use Case 1
Title: Determine License and Vulnerability Information

Primary Actor: Manager

Goal in Context: The manager is able to determine the license and vulnerability information from the given project information. 

Stakeholders: 
* Manager: To receive correct and relevant information and adjust policies accordingly. 
* Developer: To provide the relevant file and package level information. 
* Project Owner: To clearly understand the manager decisions in order to make accurate decisions on whehter or not to stop or continue the project. 

Preconditions: 
* Relevant file/package information is in the proper database.
* The proper project information has been provided. 

Main Success Scenario: The manager receives the correct license and vulnerability information for the requested software packages. 

Failed End Conditions: The manager receives the incorrect license and vulnerability information for the requested software packages. 

Trigger: Manager identifies or uploads project information to which license and vulnerability information can be provided. 

##Use Case 2
Title: Developer Upload

Primary Actor: Developer

Goal in Context: The developer is able to upload a software package to the License Scanner and have correct information sent back. 

Stakeholders: 
* Developer: To provide the software package to be uploaded to the License Scanner.
* Manager: To Receive correct information from the software package sent to the License Scanner. 
* Project owner: To clearly be able to understand the manager decisions to make a decision on whether to continue the proeject or to stop it. 

Preconditions: 
* The software package is correctly uploaded to the orchestrator. 
* The orchestrator correctly sends the software package to the License Scanner.

Main Success Scenario: The Developer successfully uploads the software package to the License Scanner and the license results sent back are accurate. 

Failed End Conditions: The Developer unsuccessfully uploads the software package to the License Scanner or the license results sent back are inaccurate. 

Trigger: The developer uploads the information to the orchestrator. 

##Use Case 3
Title: Retrieve Policy

Primary Actor: Manager

Goal in Context: The manager is able to retrieve the policy from the Policy DB. 

Stakeholders: 
* Manager: To receive accurate policy information from the database. 
* Project Owner: To clearly understand the manager's decisions to change specific policies in the company. 

Preconditions: 
* The policy name that is being sent is acutally in the database.
* The correct policy name has been provided. 

Main Success Scenario: The manager correctly receives the policy that they were intending to retrieve from the database. 

Failed End Conditions: The manager incorrectly receives the policy that they were intending to retrieve from the database. 

Trigger: Manager sends a request to the Retrieve policy info process and the policy information is sent back. 
