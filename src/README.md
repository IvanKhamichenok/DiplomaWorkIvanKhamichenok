Testing an online diary site https://my.monkkee.com/#/entries

Description:

This site is for:
- creating notes
- production of print data notes
- search for notes
- creating tags
- deleting notes

Checklist

- test authorization (valid login and password, empty, incorrect values) - UI
- test for creating a new note -UI
- note deletion test -UI
- print test and notes
- check adding tag

Stack of technologies 
- TestNG - for creating and running of tests

- Maven - for project guiding, gathering and running tests

- Selenium - for automating of interaction with web browsers

- Allure - for creating reports

- Jenkins - for running tests

- REST Assured and GSON - for automation of API tests

- Lombok and log4j - for logging

Test running
Maven: mvn clean test (-DsuiteXmlFile=src/test/resources/{}, xmlFile)

Jenkins: choose project -> build / build with parameters

Reporting
Maven: mvn clean test -> allure report -> allure serve

Jenkins: add reporting: choose project -> Configure -> Post-build actions -> Allure Report
view report: choose project -> click Allure Report on left-side menu