### CI/CD


Jenkins: 

Kawaguchi 
Hudson project - 
Sun micro systems 
Oracle bought it 
Wanted to kill it 
Oracle Fusion 


On-premises vs Cloud computing 
- Organization 
- Cloud na summa simple oru machine in remote 

Benefits
Scalability & elasticity 
Accessibility & reliability 
Cost & operational efficiency 
Rapid & flexible deployment 
Security & compatibility 

Drawbacks
- Internet connectivity 
- Financial commitment 
- Data security & protection
- Readiness & maturity 
- Interoperability 


Cloud Providers: 
- AWS
- Alibaba cloud
- Azure
- Gcloud 
- VMware
- Salesforce





Java -jar ./jenkins.war 


Git
Maven integration 
Build pipeline
Copy arifact 






Global tool config 

Step1: 
Poll scm 
Build : clean compile 

Post build action: 
Archive artifact:
**/*

Step2  n clear

Build: compiler:testCompile

Build trigger: 
Job1 

Pre steps:         \
Copy artifact from another project: 
Job1 
Artefacts to copy : job1 

Post build action: 
Archive artifact:
**/*

Step3 
Build trigger: 
Job2 

Presteps: 
Job2 
Arti facts to copy **/*

Surefire:test
