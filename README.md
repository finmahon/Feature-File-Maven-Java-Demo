# Simple BDD Demo App

## Summary

Application has Account Objects, which have an id, balance and authoritisation level, and User Objects, which have a name, password and type.  There are three valid User types: User, Supervisor and Manager.  The BDD tests set up accounts and check that: user type `user` can access accounts with auth level 0, user type `supervisor` can access accounts with auth level 1, and user type `managefr` can access accounts with auth level 2  

## Objects:

`Account` has fields: id, balance and level

`User` has fields: name, password, user type

User type `user` can access balance on accounts at level 0

User type `supervisor` can access balance on accounts at level 1 or lower  

User type `manager` can access balance on accounts at level 2 or lower


## Cucumber dependency

io.cucmber dependency added to POM to facilitate BDD testing usung feature files in `src/test/resources/com/mycompany/app`

[Maven Cucmmber](https://mvnrepository.com/artifact/io.cucumber)

[Cucumber.io](https://cucumber.io/)


## Feature Files 
defined in `src/test/resources/com/mycompany/app`

## Steps Definitions
defined in `src/test/java/com/mycompany/app/StepDefinitions.java`

## Run BDD Tests

`mvn test`

