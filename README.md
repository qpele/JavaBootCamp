# JoonasBootCamp
Boot camp project


Goal of the project is to get introduced to technologies Joonas system is using.

## Lesson 1 - GIT

### Step 1. Git basics checkout, commit, push, pull.

1. Checkout the project
2. Make change that software do not output "Hello world" but "Hello Joonas".
3. Commit and push change.

### Step 2. branching merging

1. Create a new branch from the master name it helloWorld
2. Make change in helloWorld branch: "Hello world" instead of "Hello Joonas"
3. Commit and push
4. Merge branch helloWorld into master.

### Step 3 - conflict resolution

1. On master branch change text to "Hello everybody". commit. push.
2. On helloWorld branch change text to "I'm hungy". commit. push.
3. Merge helloWorld branch into master.
4. Resolve conflict so text on master would be "I'm hungry".


## Lesson 2 - Maven

1. Setup project to be build using Maven. This also will required to proper folder structure to be created like (src/main/java/.. java packages and classes,
then src/test/java.... 
2. Move Main class to package com.igame.bootcamp
3. Install project using maven clean install. The result should be .jar file with all project files in target folder
4. Integrate maven project with your IDE so you can run maven command directly from IDE. The best way is to use it "import project from maven" 
all IDEs has this feature.
 
This is just initial maven configuration. In any following lession we will have to deal with maven. From this point all builds will be done using maven

## Lesson 3 - Slf4 and Log4J2

Log4J and his wrapped Slf4j is a tool that we are using for writing logs.
 Goal of this lesson is to have this in logs when program is executed:
 
11/Sep/2015 09:00:00,012   DEBUG  Main      - program starts
11/Sep/2015 09:00:00,012   INFO  Main      - Hello world
11/Sep/2015 09:00:00,012   DEBUG  Main      - program exits


1. Add dependency in pom.xml for most recent versions of Slf4 and Log4J2
2. Write logs using Slf4j library to default output (console) without any formatting , just plain text
3. Setup log4j2 to write logs to a file.
4. Setup log4j2 to write logs in expected format


## Lesson 4. jUnit

jUnit is Unit testing framework we are using

1. Create a method in main class: public int add(int a, int b) that will return a+b
2. Write a test that will confirm that method is working correctly.


## Lesson 5. Spring

Real stuff. All previous lesson where just preparation, now we are starting to do real stuff.

1. Create a new class HighLevelMath that will method public int add(int a, int b).
2. Change main class do to something like new HighLevelMath();log.info(" 1+1 = {}",highLevelMath.add(1,1));
3. Setup spring configuration with Annotations so HighLevelMath will become Spring bean.
4. Load spring context in Main.class and instead new HighLevelMath() get highLevelMath object from spring context.
5. Write a spring test that will load HighLevelMath object from spring context and test it.


## Lesson 6. JPA
Java Persistence API.

1. Create a table in MySQL user(id,username), id is a primary key
2. Create a JPA Domain object User that is mapped to user table
3. Write a test that will add a new user in a the database and after that read the user object from db so you can confirm that
user data are saved correctly.


## Lesson 7. Spring Data + JPA

1. Do same thing as lesson 6 but with using Spring Data JPA
https://docs.spring.io/spring-data/jpa/docs/current/reference/html/




 
 
 
 
 
 
 
 





