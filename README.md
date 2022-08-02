# git | GitHub

<h3 align="center">merge / branch</h3>

1. On the local repository, make branches for:

- Postman   --->	   ```	git branch Postman ```
- Jmeter   --->   	```	git branch Jmeter ```
- CheckLists   --->	```	git branch CheckLists ```
- Bag Reports 	```	git branch BugReports ```
- SQL 	 --->	```	git branch SQL ```
- Charles  --->	```	git branch Charles ```
- Mobile testing --->  ```	git branch MobileTesting ```

2. Push all branches to an external repository--->

 ``` git push -u origin Postman Jmeter CheckLists BugReports SQL Charles MobileTesting ```

3. In the Bug Reports branch, make a text document with the bug report structure--->

 ``` git checkout BugReports ``` --->
 ``` touch BugReports_str.txt ```  --->
 ``` vim BugReports_str.txt ``` --
```
	Bug Name:
	Bug ID:
	Area Path:
	Build Number:
	Severity:
	Priority:
	Assignet to:
	Reported by:
	Status:
	Environment:
	Derscription:
	Steps to reproduse:
       		1)
       		2)
       		3)...
	Expected Result:
	Comment:
```
 press ``` ESC ```  -> ``` SHIFT+Z+Z ```
 
 4. Push the bug report structure to the external repository --->
 
 ``` git add . ``` --->
 ``` git commit -m "added bugreport_structure.txt" ``` --->
 ``` git push ```
 
 5. Merge the Bug Reports branch into Main --->
 
 ``` git checkout main ``` --->
 ``` git merge BugReports ```
 
 6. Push main to the external repository --->
 
  ``` git push ```
  
  7. In the CheckLists branch, outline the checklist structure --->
  
 ``` git checkout CheckLists ``` --->
 ``` touch CheckLists_str.txt ``` ---> 
 ``` vim CheckList_str.txt ``` --
 ```
	ID:
	Header:
	Part of functionality:
	Test:
	Expected result:
	Test cases:
	Bug reports:
	Comment:
  ```
 press ``` ESC ```  -> ``` SHIFT+Z+Z ```
 
 8. Push the structure to an external repository --->
 
 ``` git add . ``` --->
 ``` git commit -m "added checklist_structure.txt" ``` --->
 ```git push ```


9. On the external repository, make a Pull Request of the CheckLists branch in main
10. Synchronize External and Local branches Main --->

 ``` git checkout main ``` ---> 
 ``` git fetch ``` --->
 ``` git pull ```

<h3 align="center">JSON</h3>

1. Create an external repository called JSON
 ---> In GitHub, click on the ``` New ``` button --> in the Repository name, write ``` JSON ``` -->
 make the repository public --> Add a ``` README ``` file --> Click on the ``` Create repository ``` button
 
 2. Clone the JSON repository to the local machine.
 ---> ``` git clone ``` link to the repository (in the required repository, click on the ``` Code ``` button on the right and copy ``` HTTPS ```)
 
 3. Inside the local JSON, create a “new.json” file.
 ---> ``` touch new.json ```
 
 4. Add file under git.
 ---> ``` git add new.json ```
 
 5. Commit the file.
 ---> ``` git commit -m "===" ```
 
 6. Submit the file to an external GitHub repository.
 ---> ``` git push ```
 
 7. Edit the content of the “new.json” file - write information about yourself (name, age, number of pets,
 future desired salary). Everything is written in JSON format.
 ---> ``` vim new.json ``` --> press ``` I ```
 ```json
  {
	"name": "Bezirgen Akmammedov",
	"age": 22,
	"animals": "null",
	"salary": "2500 $"
 }
 ```
 press ``` ESC ``` -> ``` SHIFT+Z+Z ```
 
 8. Push changes to an external repository.
 ---> ``` git add new.json ``` --> ``` git commit -m "===" ``` --> ``` git push ```
 
 9. Create preferences.json file
 ---> ``` touch preferences.json ```
 
 10. Add information about your preferences to the preferences.json file (Favorite movie, favorite series, favorite food, favorite season,
 country you would like to visit) in JSON format.
 ---> ``` vim preferences.json ``` --> press ``` I ```
 ```json
 {
	"movie": "Interstellar",
	"show": "One Piece",
	"food": "Manti",
	"season": "Autumn",
	"country": "South Korea"
 }
 ```
 press ``` ESC ``` -> ``` SHIFT+Z+Z ```
  
   11. Create a file sklls.json add information about the skills that will be studied in the course in JSON format 
 ---> ``` touch skills.json ``` --> ``` vim skills.json ``` --> press ``` I ```
 ```json
 {
	"skills": "Linux, Github, Postman, Jmeter, SQL, Charles"
 }
 ```
  press ``` ESC ``` -> ``` SHIFT+Z+Z ```
  
  12. Send 2 files at once to an external repository.
 ---> ``` git add . ``` --> ``` git commit -m "===" ``` --> ``` git push ```
 
 13. On the web interface, create the bug_report.json file.
 ---> in the JSON repository click on the ``` ADD FILE ``` button --> creat new file
 
 14. Make Commit changes (save) changes on the web interface.
 ---> fit at the bottom of the page
 
 15. Modify the bug_report.json file on the web interface, add a bug report in JSON format.
 ---> in the JSON repository we find the desired file and click on its name --> on the right click on the pencil icon (edit) -->
  ```json
  {
      "Bug Name": "Application crashes upon clicking the SAVE button while creating a new user",
      "Bug ID": "(It will be automatically created by the BUG Tracking tool once you save this bug)",
      "Area Path": "USERS menu-> New Users",
      "Build Number": "Version Number 3.0.1",
      "Severiy": "High",
      "Priority": "High",
      "Assignet to": "Developer-name",
      "Reported By": "Bezirgen",
      "Reported On": "09-June-2022",
      "Reason": "Defect",
      "Status": "New/Open/Active(Depends on the Tool you are using)",
      "Environment": "Windows 10",
      "Description": "Application crashes upon clicking the SAVE button while creating a new the user, hence unable to create a new user in the application",
      "STR1": "Login into the Application",
      "STR2": "Navigate to the Users Menu -> New User",
      "STR3": "Filled out all the user information fields",
      "STR4": "Clicked on the ‘Save’ button",
      "STR5": "Seen an error page 'ORA1090 Exception: Insert values Error…'",
      "STR6": "See the attached logs for more information (Attach more logs related to the bug..IF any)",
      "STR7": "Also see the attached screenshot of the error page",
      "Expected Result": "On clicking the SAVE button, you should be prompted to a successful message 'New User has been created successfully'"
 }
```

16. Make Commit changes (save) changes on the web interface.
 ---> click on the ``` Commit changes ``` button below (save)
 
 17. Synchronize external and local JSON repository
 ---> ``` git pull ``` (in terminal)
  
<h3 align="center">XML</h3> 

1. Create an external repository called XML.
 ---> In GitHub, click on the ``` New ``` button --> in the Repository name, write ``` XML ``` -->
 make the repository public --> Add a ``` README ``` file --> Click on the ``` Create repository ``` button
 
 2. Clone the XML repository to the local machine.
 ---> ``` git clone ``` link to the repository (in the required repository, click on the Code button on the right and copy ``` HTTPS ```)
 
 3. Inside the local XML, create the “new.xml” file.
 ---> ``` touch new.xml ```
 
 4. Add file under git.
 ---> ``` git add new.xml ```
 
 5. Commit the file.
 ---> ``` git commit -m "===" ```
 
 6. Submit the file to an external GitHub repository.
 ---> ``` git push ```
 
 7. Edit the content of the “new.xml” file - write information about yourself (name, age, number of pets,
 future desired salary). Everything is written in XML format.
 ---> ``` vim new.xml ``` --> press ``` I ```
 
```xml
<INFO>
	<name>Bezirgen Akmammedov</name>
	<age>22</age>
	<animal>null</animal>
	<salary>2500$</salary>
</INFO>
```
press ``` ESC ``` -> ``` SHIFT+Z+Z ``` 
  
 8. Push changes to an external repository. 
 ---> ``` git add new.xml ``` --> ``` git commit -m "===" ``` --> ``` git push ```
 
 9. Create preferences.xml file
 ---> ``` touch preferences.xml ``` 
 
 10. Add information about your preferences to the preferences.xml file (Favorite movie, favorite series, favorite food, favorite season,
 country you would like to visit) in XML format. 
 ---> ``` vim preferences.xml ``` --> press ``` I ```
 
 ```xml
 <PREFERENCES>
	<movie>Interstellar</movie>
	<show>One Piece</show>
	<food>Manti</food>
	<country>South Korea</country>
</PREFERENCES>
 ```
 press ``` ESC ``` -> ``` SHIFT+Z+Z ```  
 
 11. Create a skills.xml file add information about the skills that will be studied in the course in XML format
 ---> ``` touch skills.xml ``` --> ``` vim skills.xml ``` --> press ``` I ``` 
 
 ```xml
 <SKILLS>
	<skills>Linux, Github, Postman, Jmeter, SQL, Charles</skills>
</SKILLS>
 ```
  press ``` ESC ``` -> ``` SHIFT+Z+Z ```
  
  12. Send 2 files at once to an external repository.
 ---> ``` git add . ``` --> ``` git commit -m "===" ``` --> ``` git push ```
 
 13. On the web interface, create a bug_report.xml file
 ---> in the xml repository click on the ``` ADD FILE ``` button --> creat new file
 
 14. Make Commit changes (save) changes on the web interface.
 ---> fit at the bottom of the page
 
 15. Modify the bug_report.xml file on the web interface, add a bug report in XML format.
 ---> in the XML repository we find the desired file and click on its name --> on the right click on the pencil icon (edit) -->
 
 ```xml
 <BUGREPORT>
  <BugName>Application crashes upon clicking the SAVE button while creating a new user</BugName>
  <BugID>(It will be automatically created by the BUG Tracking tool once you save this bug)</BugID>
  <AreaPath>USERS menu -> New Users</AreaPath>
  <BuildNumber>Version Number 3.0.1</BuildNumber>
  <Severity>High</Severity>
  <Priority>High</Priority>
  <AssignetTo>Developer-X</AssignetTo>
  <ReportedBy>Bezirgen</ReportedBy>
  <ReportedOn>09-June-2022</ReportedOn>
  <Reason>Defect</Reason>
  <Status>New/Open/Active(Depends on the Tool you are using)</Status>
  <Environment>Windows 10</Environment>
  <Description>Application crashes upon clicking the SAVE button while creating a new the user, hence unable to create a new user in the application</Description>
  <STR1>Login into the Application</STR1>
  <STR2>Navigate to the Users Menu -> New User</STR2>
  <STR3>Filled out all the user information fields</STR3>
  <STR4> Clicked on the ‘Save’ button</STR4>
  <STR5>Seen an error page “ORA1090 Exception: Insert values Error…”</STR5>
  <STR6>See the attached logs for more information (Attach more logs related to the bug..IF any)</STR6>
  <STR7>Also see the attached screenshot of the error page</STR7>
  <ExpectedResult>On clicking the SAVE button, you should be prompted to a successful message “New User has been created successfully”</ExpectedResult>
</BUGREPORT>
 ```
 16. Make Commit changes (save) changes on the web interface.
 ---> click on the ``` Commit changes ``` button below (save)
 
 17. Synchronize external and local XML repository
 ---> ``` git pull ``` (in terminal)
 
 
 
