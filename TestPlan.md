# Test Plan


**Author**: Team 11

## 1 Testing Strategy

### 1.1 Overall strategy

The testing process include different phrases:

a. Unit testing

The unit testing will be based on each class in the project. It will be going on while the development is being worked on. The developer will perform unit testing on each class to ensure it functions as expected once it is built. In this process, the classes will mainly be tested independently of each other and basic functionality will be the main focus. 

b. Integration testing

Integration testing will check how the classes/modules function interactively. The focus will be on the classes that work in a combined or integreated way. The QA analyst will take the main responsibility to use test cases to verify different classes work together well. The QA analyst will also track the inputs and outputs closely and work with the developer for any necessary investigation.


c. System testing

The system testing will check all the units as a complete and integrated software. The QA analyst will perform the system testing when all the classes have been developed and the previous steps of testing have been completed.


d. Regression testing

The regression testing will confirm any change to the code would not cause any issues to other existing units or functions. Once a change is made to the code, the QA analyst will use the same use cases from previous steps to validate the change will bring about positive testing results. 



### 1.2 Test Selection

All the four testing levels discussed above will be performed. The black-box method will be used for all the four levels to ensure the software works as expected. In the meantime, white-box techniques may be used by the developer for some detailed logic check or process check, especially in the levels of unit testing or even integration testing. Test cases would be created for each use case in the use case model. Also different input/precondition combinations would be verified to make sure all scenarios are covered. Unit tests are needed to thoroughly cover each individual class and function.



### 1.3 Adequacy Criterion

Functional testing will be the main form of testing throughout the phrases of our testing. Its main goal is to make sure the functionality requirements are met. Structural testing may be used to perform logic check by the developer, especially in the phrase of unit testing and integration testing.



### 1.4 Bug Tracking

Once a bug is detected or identified, the result will be recorded in the Github repository. The developers and QA analysts will work together to address the issues. And a new round of unit testing, integreation testing and regression testing will be conducted to ensure the software quality.



### 1.5 Technology

JUnit will be the primary tool for the testing considering its automated and streamlined process. Other tools may be needed as the project progresses.


## 2 Test Cases


| ID  | Purpose | Steps | Expected result | Actual result | Passed or failed |
|---|---|---|---|---|---|
| 1 | Create new user | Verify unique username, add username email, assign user type | The username of the new user is unique; both username and email added; user should be either administrator or player |  |  |
| 2 | Log in | Verify user can log in and displays after log-in are as expected | New user can log into the game; main menu displayed for player; cryptogram statistics displayed to administrator |  |  |
| 3 | Log out | Allow a logged in player to log out | Player is not longer logged in; player is viewing the login screen |  |  |
| 4 | View player score list | Verify the list of all players and their information is shown to player in descending order of points | Player can see a list of all players sorted by descending number of points, including their username, points and number of attempted cryptograms |  |  |
| 5 | Create cryptogram | Allow the player to create a new cryptogram for other players to attempt | The new cryptogram has been added to the collection of available cryptograms; the player has recieved confirmation that it was successfully created; the player is viewing the main menu |  |  |
| 6 | Solve a Random Cryptogram | Verify the player is shown a cryptogram and is allowed to attempt to solve it | The player has either: (1) solved the cryptogram (2) run out of attempts (3) Left the cryptogram unsolved and returned to the menu; the number of attempts, the scores and the messages are properly changed |  |  |
| 7 | View list of cryptogram statistics | Verify the administrator can access the list of cryptogram statistics | The administrator can see the list of cryptogram statistics |  |  |
| 8 | View cryptogram details | Verify the administrator can view the details of a cryptogram | The administrator can see the details of the selected cryptogram |  |  |
| 9 | Disable cryptogram and penalize creator | Verify the administrator is able to disable a cryptogram and penalize the creator | The cryptogram can be disabled; the creator of the cryptogram is penalized by the number of points specified by the administrator (between 0 and 10) |  |  |



