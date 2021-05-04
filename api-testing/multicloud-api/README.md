# API Testing Automation Framework

**Introduction**

This framework has developed in [JUNIT](https://junit.org/) using [Gradle](https://gradle.org/) Build tool.
Currently added for multicloud project of soda foundation. Later it could be reused for other projects.
Junit framework details [Link](https://www.tutorialspoint.com/junit/index.htm)

**Why this?**

Junit is widely used testing framework along with Java Programming Language. You can use this automation framework for both unit testing and UI testing.
You will get test report in html format which will help developer to test their code and to identify bugs.

**How to install and use?**<br/>
    For testing purposes you can deploy OpenSDS refering to [OpenSDS Cluster Installation through Ansible](https://github.com/sodafoundation/api/wiki/SODA-Projects-Cluster-Installation-through-Ansible). <br/>
 Java 8 is required to run [IntelliJ IDEA](https://intellij-support.jetbrains.com/hc/en-us/articles/206544879-Selecting-the-JDK-version-the-IDE-will-run-under) <br/>
 Download Intellij idea community edition tool and install in your pc.
 [link](https://www.jetbrains.com/idea/download/#section=windows)
 
 Click on File > Open or  You Can create new Project click on File > Project
 
 Get a project from version control [Link](https://www.jetbrains.com/help/idea/import-project-or-module-wizard.html)
 
 Build Project:<br/>
 From the main menu, select Build | Rebuild Project for the entire project. [Link]( https://www.jetbrains.com/help/idea/compiling-applications.html)

**How to add tests?**

 In [Project structure](https://docs.gradle.org/current/userguide/organizing_gradle_projects.html) `src\test\java` write your own test case and 
 `src\main\java` write here your business logic now [Run](https://www.jetbrains.com/help/idea/running-applications.html).
 
 **How to set environment variable in intellij?**
   
   Before test execute setup this environment variables select [Run | Edit Configuration](https://www.jetbrains.com/help/idea/creating-run-debug-configuration-for-tests.html) from the main menu and set variables.
   
   For CreateBucketBackendTest and LifecycleTests set following variable <br/>
  `HOST_IP=***.***.*.***;INPUT_PATH=D:/SODA-Test (Your Project Folder Path);API_SERVER_PORT=:****;S3_API_PORT=:****`
   
   For MigrationTests set following variable <br/>
  `HOST_IP=***.***.*.***;INPUT_PATH=D:/SODA-Test (Your Project Folder Path);API_SERVER_PORT=:****;S3_API_PORT=:****;SCHEDULE_TIME=00 00 07 29 5 5` 

