Java Play Rest Data Services

This sample application demonstrates how to write a database backed Java Web application (powered by WebSphere Liberty) and deploy it on Bluemix.

Files

*   javaplay-rest-dataservices.war

    This WAR file is actually the application itself. It can be deployed on WebShpere Liberty application server either manually or via CF client push command.
    Every time your application code is updated, you'll need to regenerate this WAR file and push to Bluemix again. See the next section on detailed steps.
    You don't need this file if you are deploying this application using eclipse Bluemix deployment tools.
    
*	manifest.yml

	This is the manifest file for CF push command.
	You don't need this file if you are deploying this application using eclipse Bluemix deployment tools.
    
*   WebContent/

    This directory contains the client side code (HTML/CSS/JavaScript) of your application as well as compiled server side java classes and necessary JAR libraries.
    
*   src/

    This directory contains the server side code (JAVA) of your application. In this simple starter application, there's only one class: 'com.ibm.cloudoe.samples.HelloResource'
    
*   build.xml

    This file allows you to easily build your application using Ant.
    
*	dep-jar/

	This directory contains libraries that are needed to compile locally, but are provided by Bluemix and not included in the WAR file. 

Usage

This is an example of web REST application that translates user REST calls into underlying data services API calls and returns the result. Only few methods are implemented to illustrate how developer can do similar application.
This application works as is and can be deployed to Bluemix or any other WebSphere Liberty application server. The deployment can be done either via CF push command or via eclipse Bluemix tools.
Developers can use this sample in following ways:
1. Fork the original project repository: https://github.com/ibmecod/javaplay-rest-dataservices. Then update this code by modifying existing and adding new functionality, services, etc.
2. Check out the project and copy classes/resources in whole or partially for use in their projects.
3. Follow the code and presentation to understand application architecture and data flow then reproduce same architecture pattern in their project.
