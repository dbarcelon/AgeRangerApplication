# AgeRangerApplication
Age Ranger Application Technical Exam

I have implemented the Age Ranger Application by using AngularJS Version 1.x as the client interface and ASP.Net Web API as the back-end tier to connect to the database using C#, LinQ, SQLLite

The solution contains 6 projects:

1.	AgeRanger – This project contains the client interface which uses AngularJS, Bootstrap, HTML5, CSS3, JQuery to implement Age Ranger UI
  Prerequisite:
  
    To able to run the project I used npm, node.js, bower, gulp
      a.	Please download first the npm and node.js
      
      b.	I used npm to install bower and gulp by entering the command below in npm console
      
          npm install -g bower
          
          npm install -g gulp
          
      c.	After downloading the said tools, I used “bower” to download the components that I define in “bower.json” that was needed in the project by entering the command below:
          bower install
      d.	I used “gulp” to run the client interface in node.js server by entering the command below:
          gulp serve
2.	AgeRanger.API – This project contains the definition of Web API controllers that will be call by the client interface.  Please run the NUget Package Manager to download the dependency components to run the project which was defined in "packages.config"
3.	AgeRanger.Business - This project contains the business logic of the system that will handle the data validation and data processing. This was called by “AgeRanger.API”
4.	AgeRanger.Data – This project contains the definition of data model, data repository and handling the data connection to the database. This was called by “AgeRanger.Business” for data manipulation
5.	AgeRanger.Utils – This project contains the ad-hoc utilities that were used by the system such as event logging to identify easily why the system does not successfully run or why the record was not added.
6.	AgeRanger.API.Tests – This project contains the unit testing for the project “AgeRanger.API”
