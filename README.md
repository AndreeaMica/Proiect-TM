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
    
     3.4 Daily test summary reports
    
     3.5 Traceability matrix
    
     3.6 Test case results
    
     3.7 Bugs report
    
     3.8 Test completion report

## 1. Introduction
    
This test plan describes the strategies, process, workflows and methodologies used to plan, organize, execute and manage testing process for OrangeHRM browser application, Job section from Admin Module.

   ### 1.1   Project Objective 

    
The scope of the final project for ITF Manual Testing Course is to use all gained knowledge through the course and apply them in practice using a live application.
    
Application under test: [OrangeHRM](https://opensource-demo.orangehrmlive.com/web/index.php/auth/login)
    
Application documentation: [OrangeHRM.pdf](https://github.com/AndreeaMica/Proiect-TM/blob/main/Complete-Administrative-User-Guide.pdf)
    
   Tools: Jira, Zephyr Squad, Postman, MySql
    
   ### 1.2 Functionalities in scope
   
   - The 'Job' section of Admin module which is defined in software requirement specs need to be: functional testing, GUI testing, API testing
   - Screenshots from Jira with user story details here [User story 1](https://github.com/AndreeaMica/Proiect-TM/blob/main/OP-3.pdf)
     [User story 2](https://github.com/AndreeaMica/Proiect-TM/blob/main/OP-24.pdf)
     
    
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
    
| Roles | Responsible   |
| :---: | :---: |
| Product Owner | Michael Bitter| 
| Project Manager  | Jamer Koors| 
| Sofware Developer | Andrew Rootman| 
| QA Engineer | John Raspberry|
| Senior QA Engineer | Andreea Moldovan|
   
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
   -    Product risk: functional and non functional errors
     
   ### 2.2 Test analysis
    
   -    Analyse business requirements to make sure that we have all the details for creating the test conditions
   -    The testing process will be executed based on the above requirements for the 'Job' section of the Admin Module. 
    
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
       -    Verify that admin user can cancel editing a pay grade name 
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
    
Based on the analysis of the specifications, the test design techniques used for generating test cases are boundary value analisys, equivalence partitioning and use case testing.
    
   ### 2.4 Test implementation
    
Verify that the following elements are ready before the test execution phase:
    
   -    Test environment is up and running: [OrangeHRM](https://opensource-demo.orangehrmlive.com/web/index.php/auth/login)    
   -    Acces to the environment is given username: Admin, password: admin123    
   -    Cycle summary was created and test cases were added to the Cycle Summary    
   -    Postman collection were created
    
   ### 2.5 Test execution
    
   -    Test cases were executed from the created Cycle Summary
   -    Bugs were created based on the failed test cases    
   -    API test cases were executed    
   -    Full regression pack was executed
    
   ### 2.6 Test completion
    
 As the Exit criteria were met and satisfied as mentioned in the appropriate section, this feature is suggested to ‘Go Live’ by the Testing team.
    
   ### 2.7 Test monitoring and control
    
   -   Generate periodic reports to check the project status for the executed test cases and status for the converge of the business requirements.        
   -   Traceability matrix was generated    
   -   Test execution was generated, the final report shows that a number of 7 tests have failed of a total of 21 tests.     
   -   A number of 21 test cases were planned for execution and all of them were executed    
   -   A number of 7 bugs were found, from which the priority is high and medium.

First week report ![raport intermediar orangehrm](https://github.com/AndreeaMica/Proiect-TM/assets/128214596/ca8bd967-b432-49bb-a55a-466932656f46)

Second week report ![raport intermediar 2 orangehrm](https://github.com/AndreeaMica/Proiect-TM/assets/128214596/eb9a4102-3d39-43ab-9e53-386e213875c0)

    
## 3. Test deliverables

   ### 3.1 Test plan

   The test plan should be delivered to the Project Manager until the 5th week of the TM Courses of the ITF Company.
    
   ### 3.2 Test conditions

   [Test conditions](https://github.com/AndreeaMica/Proiect-TM/blob/main/test%20conditions%201.png)
   
   [Test conditions](https://github.com/AndreeaMica/Proiect-TM/blob/main/test%20conditions%202.png)
   
   [Test conditions](https://github.com/AndreeaMica/Proiect-TM/blob/main/test%20conditions%203.png)
   
   [Test conditions](https://github.com/AndreeaMica/Proiect-TM/blob/main/test%20conditions%204.png)
    
   ### 3.3 Test cases

   You can find the test cases and steps [here](https://github.com/AndreeaMica/Proiect-TM/blob/main/OP-26-combined.pdf)
    
   ### 3.4 Daily test summary reports

   [Test report1](https://github.com/AndreeaMica/Proiect-TM/assets/128214596/ca8bd967-b432-49bb-a55a-466932656f46)
   [Test report2](https://github.com/AndreeaMica/Proiect-TM/assets/128214596/eb9a4102-3d39-43ab-9e53-386e213875c0)
    
   ### 3.5 Traceability matrix

   Here you can find the [traceability matrix](https://github.com/AndreeaMica/Proiect-TM/blob/main/Forward%20Traceability%20Matrix.xlsx)
    
   ### 3.6 Test case results

   You can find the test case results [here](https://github.com/AndreeaMica/Proiect-TM/blob/main/OP-26-combined%20(1).pdf)
    
   ### 3.7 Bugs report
    
   The first bug report has medium impact, it allows saving a paygrade without adding a minimum and maximum salary.
   [Bug 1](https://github.com/AndreeaMica/Proiect-TM/blob/main/BUG1.png)

   Second bug report has high impact because the 'Job title' field is disabled and cannot add any job title.
   [Bug 2](https://github.com/AndreeaMica/Proiect-TM/blob/main/BUG2.png)

   Third bug report allows to add special characters in 'Job title' field instead of showing an error message.
   [Bug 3](https://github.com/AndreeaMica/Proiect-TM/blob/main/bug3.png)

   The fourth bug report shows that a combination of numbers and letters can be added in 'Job title' field, instead of showing an error message.
   [Bug 4](https://github.com/AndreeaMica/Proiect-TM/blob/main/bug4.png)

   The fifth bug report shows that cannot save multiple currencies, despite of given documentation.
   [Bug 5](https://github.com/AndreeaMica/Proiect-TM/blob/main/bug7.png)

   
   [Bug 6](https://github.com/AndreeaMica/Proiect-TM/blob/main/bug8.png)
   [Bug 7](https://github.com/AndreeaMica/Proiect-TM/blob/main/bug9.png)
    
   ### 3.8 Test completion report

   [test completion](https://github.com/AndreeaMica/Proiect-TM/blob/main/raport%20general.png)
    
   ### 3.9 Schedule


| Date | Task   | Executed by   | 
| :---: | :---: | :---: | 
| 11.03.2003 | Run functional test cases for Job submenu    | Andreea Moldovan    | 
| 18.03.2023 | Run GUI testing for Job title submenu    | Andreea Moldovan      |
| 22.03.2023 | Run GUI testing for Pay Grades submenu    | Andreea Moldovan    |
| 15.04.2023 | Run functional testing for Pay Grades submenu     | Andreea Moldovan      |
| 28.05.2023 | Export daily report     | Andreea Moldovan      |
| 16.07.2023 | Export traceability matrix      | Andreea Moldovan      |
| 10.08.2023 | Export general report       | Andreea Moldovan      |
| 20.08.2023 | Send final project       | Andreea Moldovan      |


   
   
    


