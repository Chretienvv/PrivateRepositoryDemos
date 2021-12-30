This public repository demo's the project that are in my private repository for security reasons. This is my way of showing you the work I made.
Currently I am working on a new portfolio website. This is a temporary way of showing you my work. 
For most Aegon projects it shows you parts of the AWS architecture. I was the Frontend developer for Matroesjka, Racetrack and Developer portal.

What you will find in this repository:

### SoPickMeUp Project overview
SoPickMeUp is a carpool web app that makes it possible for Sogetists to ride together to events and training. This makes the journey more fun, more efficient, and more environmentally conscious. In a team of developers and designers I acted as frontend developer and scrum master. This with CSR, security and AVG always in mind.

Techniques: Angular, Cascading Style Sheets (CSS), Front-end development, GIT, Bootstrap HTML, REST, TypeScript, Unit testing

### Aegon Cost dashboard
A cloud dashboard that calculates the cost for Aegon Teams inside AWS.  The end product is an costdashboard that is used by the financial responsibles every day.
    
Techniques: TypeScript, AWS, Python


### InnoSportlab project overview
For InnoSportLab de Tongelreep I worked on “The smart swimming sensor app”. This innovation project was set up with a team of Sogeti colleagues. The purpose of the application is to analyse swimmers' training and forward this data to the swimmer.
    
Techniques: Agile/Scrum, Cascading Style Sheets (CSS), Front-end development, HTML, Ionic, JSON, Mobile development, TypeScript


### Hawkeye
Aegon Hawkeye is a monitoring tool create by the Cloud Platform Management team to help other teams to stay within Aegon compliancy.  
It continuously monitors AWS resources and alerts the teams when a resource gets out of compliance. After a configurable amount of time, the system also alerts Aegon Security non-compliant resources are within the AWS environment.

Techniques: TypeScript, AWS, Python

### Longrunner proces
Made a generic pattern that multiple aegon teams use to solve the lambda chaining problems. It is a cdk stack that can run with only changing the variable for the team.
Techniques: TypeScript, AWS, Python

### Matroesjka
A website that shows the ghost resources and cloudformation stacks within AWS accounts. The logic checks for the following aspects:
IP lookup- Given a specific IP, this endpoint will return matching origin networks within AegonNL accounts.
Anomaly detection -> Without having to invoke a single API, we've built some anomaly detection capabilities into Matroesjka. We pull data from MetaCloud 	 daily, and for all accounts, check whether there has been any significant increase in the amount of resources spun up. If this is the case, we'll send a 	  notification to the appropriate email address(es).
Application lookup - This is an experimental endpoint, which currently performs on a best-effort basis. In the future, we'll be able to more accurately 	supply applications running in an account based on the so called CMDB ID. Until that time, we'll try to supply meaningful information with the limited data.

Techniques: HTML, CSS, JavaScript, Python, AWS, REST

### RaceTrack
A website for RTE's and scrummasters to insert their sprint data in a central place.
Techniques: HTML, CSS, JavaScript, Python, AWS

### Developer portal
A website for the developers in Aegon to see specific Aegon rules in AWS.
Techniques: HTML, CSS, JavaScript, Python, AWS
