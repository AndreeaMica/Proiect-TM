# <h1 align="center">OrangeHRM Project<h1>
## <h1 align="center">- Test Plan -<h1>

## **Revision History**
| Date | Version   | Author   | Comments |
| :---: | :---: | :---: | :---: |
| 11.03.2003 | v1.0    | Andreea Moldovan    | Draft Plan |
| 18.03.2023 | v1.1    | Ioana Popescu      |Test result for functional testing |
| 22.03.2023 | v1.2    | Teodora Maria      |More details added for Test Implementation |

    
1. Introduction
    
     1.1 Project Objective
    
     1.2 Functionalities in scope
        
     1.3 Functionalities and tests out of scope
    
2. Test process
    
     2.1 Test planning
     
      2.1.1 Roles and responsabilities
    
      2.1.2 Entry Criteria
    
      2.1.3 Exit Criteria
    
      2.1.4 Risk detected
    
     2.2 Test analysis
    
     2.3 Test design
    
     2.4 Test implementation
    
     2.5 Test execution
    
     2.6 Test completion
    
     2.7 Test monitoring and control
    
3. Test deliverables

     3.1 Test plan
    
     3.2 Test conditions
    
     3.3 Test cases
    
     3.4 daily test summary reports
    
     3.5 Traceability matrix
    
     3.6 Test case results
    
     3.7 Bugs report
    
     3.8 Test completion report

## 1. Introduction
    
This test plan describes the strategies, process, workflows and methodologies used to plan, organize, execute and manage testing process for OrangeHRM browser application.

   ### 1.1   Project Objective 

    
The scope of the final project for ITF Manual & Automation Testing Course is to use all gained knowledge through the course and apply them in practice using a live application.
    
Application under test: [OrangeHRM](https://opensource-demo.orangehrmlive.com/web/index.php/auth/login)
    
Application documentation: [OrangeHRM.pdf](https://github.com/AndreeaMica/Proiect-TM/blob/main/Complete-Administrative-User-Guide.pdf)
    
   Tools: Jira, Zephyr Squad, Postman, MySql
    
   ### 1.2 Functionalities in scope
   
   - The 'Job' section of Admin module which is defined in software requirement specs need to be: functional testing, GUI testing, API testing
   - Screenshots from Jira with user story details
    
   ### 1.3 Functionalities and tests out of scope
    
   -	All OrangeHRM features except Admin module.
   -	Non-functional testing like stress, performance is beyond scope of this project.
   -	No QA support for mobile application developed. Only web application will be tested.
   -	Automation testing is beyond scope.  

## 2. Test process
    
   ### 2.1 Test planning
    
The Test Plan in designed to describe all details of testing for 'Job' section of the Admin Module from the OrangeHRM application.

The plan identifies the items to be tested, the features to be tested, the types of testing to be performed, the personnel responsable for testing, the resources and the schedule required to complete testing and the risk associated with the plan.
    
   #### 2.1.1 Roles and responsabilities
    
| Roles | Responsible   |    |  |
| :---: | :---: | :---: | :---: |
| Product Owner | Michael Bitter    | 
| Project Manager  | Jamer Koors   | 
| Sofware Developer | Andrew Rootman   | 
| QA Engineer | Andreea Moldovan   |
   
   #### 2.1.2 Entry Criteria
    
   -	Functional specifications defined
   -	Roles needed for the project are allocated
   -	Initial project risks were detected and mitigated
    
   #### 2.1.3 Exit Criteria 
    
   -    All tests cases have been executed 
   -    The number of unresolved bugs is insignificant or have a low priority 
   -    All resolved bugs have been re-tested and closed by QA team
   -    Deadline was reached
   -    No major risks detected remained un-mitigated
    
   #### 2.1.4 Risk detected
    
   -    Project risk: lack of experience of the QA team, short deadline of Zephyr Squad and Jira Tools, unavilability of the test environment
   -    Product risk: validation constrains on the fields might be too restrictive to the end-user
    
   ### 2.2 Test analysis
    
   -    Analyze business requirements to make sure that we have all the details for creating the test conditions
   -    The testing process will be executed based on the above requirements for the 'Job' section of the Admine Module. 
    
    The following test conditions were found:

   -    Verify that Admin user can add a job title
   -    Verify that Admin user can add multiple job titles
   -    Verify that Admin user can delete a job title
   -    Verify that Admin user can delete multiple job titles
   -    Verify that 'Job Title' field is a mandatory field
   -    Verify that Admin user can add a random number in the 'Job title field' 
   -    Verify that Admin user cannot add special characters in the 'Job title' field
   -    Verify that Admin user can add a job title with 80 characters
   -    Verify that a combination of numbers and characters is not allowed in the "job title" field
   -    Verify that the 'Job title' field from OrangeHRM app is completely visible in Chrome browser
   -    Verify that the 'Job title' field from OrangeHRM app is completely visible in Mozzilla Firefox browser when click on Add button
   -    Verify that the field 'name' is mandatory in Pay Grades section
   -    Verify that admin user can cancel editing a pay grade name after saving it
   -    Verify that admin user can edit details of a particular currency
   -    Verify that admin user can save a positive value in minimum salary field
   -    Verify that admin user cannot save a negative value in minimum salary field
   -    Verify that admin user cannot save non-numerical characters in the 'minimum salary' field
   -    Verify that the 'minimum' and 'maximum' salary fields are mandatory in the Add Pay Grade section
   -    Verify that admin user can assign multiple currencies
   -    Verify that admin user can delete multiple currencies
   -    Verify that admin user can edit a pay grade name 
    
    
   ### 2.3 Test design
    
   -    Functional test cases were created in Zephyr Squad    
   -    GUI test cases were created in Zephyr Squad    
   -    API test cases will be created in Postman
    
Based on the analisys of the specifications, the test design techniques used for generating test cases are boundary value analisys, equivalence partitioning and use case testing.
    
   ### 2.4 Test implementation
    
Verify that the following elements are ready before the test execution phare:
    
   -    Test environment is up and running: [OrangeHRM](https://opensource-demo.orangehrmlive.com/web/index.php/auth/login)    
   -    Acces to the environment is given username: Admin, password: admin123    
   -    Cycle summary was created and test cases were added to the Cycle Summary    
   -    Postman collection were created
    
   ### 2.5 Test execution
    
   -    Test cases are executed on the created on the Cycle Summary
   -    Bugs were created based on the failed test cases    
   -    API test cases were executed    
   -    Full regression pack was executed
    
   ### 2.6 Test completion
    
 As the Exit criterias were met and satisfied as mentioned in the appropriate section, this feature is suggested to ‘Go Live’ by the Testing team.
    
   ### 2.7 Test monitoring and control
    
   -   Generate periodic reports to check the project status for the executed test cases and status for the converge of the business requirements.        
   -   Traceability matrix was generated    
   -   Test execution was generated, the final report shows that a number of X tests have failed of a total of X tests.     
   -   A number of X test cases were planned for execution and all of them were executed    
   -   A number of X bugs were found, from which the priority
    
## 3. Test deliverables

   ### 3.1 Test plan
    
   ### 3.2 Test conditions
    
   ### 3.3 Test cases
    
   ### 3.4 Daily test summary reports
    
   ### 3.5 Traceability matrix
    
   ### 3.6 Test case results
    
   ### 3.7 Bugs report
    
   ### 3.8 Test completion report
    
   ### 3.9 Schedule
    
   
   
    


