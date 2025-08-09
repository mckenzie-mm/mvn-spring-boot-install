# mvn-spring-boot-install

## Installation instructions for ubuntu (Aug 2025)

I could not find a single source that worked directly without change. The following is a combination of these two websites

* https://www.alessioligabue.it/en/blog/install-spring-boot-ubuntu-complete-guide

* https://www.linode.com/docs/guides/how-to-deploy-spring-boot-applications-nginx-ubuntu-22-04/

**************************************************************************************************

### Install the Java JDK

From a command line terminal execute the followiing

```
sudo apt update

sudo apt install default-jdk
```

Then check the version to confirm the installation was a success.

```
java -version
```

### Install Maven

```
sudo apt-get install maven
```

### Install SDKMAN 

SDKMAN is used for installing Spring Boot CLI module

First get the source code with curl

```
curl -s https://get.sdkman.io | bash
```

Then run the following command from a command line terminal WITHOUT using sudo, to install SDKMAN

```
source "/home/userdir/.sdkman/bin/sdkman-init.sh"
```
In the above command, replace "userdir" with the name of your home dir.

To install Spring Boot CLI module using SDKMAN execute the following

```
sdk install springboot
```

************************************************************************************************

## Run the Spring Boot Application:

https://1kevinson.com/how-to-run-a-spring-boot-app-with-maven-command/

Navigate to the root directory of your Spring Boot project 

Execute the following Maven command to launch your Spring Boot application:

```
mvn spring-boot:run
```

This will launch a Tomcat Server on localhost:8080.
