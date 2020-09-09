# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

#### *For **both** a VM or App Service solution for the CMS app:*
- ####*Analyze costs, scalability, availability, and workflow*
    ***Cost*** - \
    VM has more cost than app service, using app servie is better.
    As per the azure pricing calculator, 1 Instance of app service running 730 hours with 10 gb storage and 1.75 gb RAM with 2 Cpu Cores is costing aroung $54.75. But For VM with 2 CPU Cores it is costing me around 152$.
    ***Scalability*** - \
    Both are scalable but, the apps need to be redeployed after scaling up/down in case of VM. This is not the case with App Service, we dont have to restart the apps while scaling while scaling up and down. We can deploy multiple apps in App Service but in one VM Server we can only deploy one app.
    ***Availability -*** \
    VM deployed app run simultaneously at 2 regions at a time, making it available 99.95% available. In App service it depends if we have multiple instances activated or not and also if they are in different regions.Even the deplyements are much faster in App service, so down time is less and app can become easily and quickly available.
    ***WorkFlow -*** \
    *VM* - It is basically IaaS (Infrastructure as a Service). Thus, Developer needs to set up most of the things, like firewalls, runtimes, compilers etc.
    *App Service* - It is Paas (Platform as a service). The user Developer just needs to create the app. Rest all things are provided.

#### *Choose the appropriate solution (VM or App Service) for deploying the app*
   App Service
- #### *Justify your choice*
    App Service is a better choice since i found it easy to use, the cost was also less and it got easliy configured with my VsCode and application management and deployement got easy and automated.

### Assess app changes that would change your decision.
*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 
 
Generally, Virtual machines are slow than actual machines. Also cost of esatblishing a server is very high, setting up all the infra is very high if we dont have cloud.
 
Maintaing the App Service is much easire as compared to the VM's. Even the App Service are much faster then the VM's, it is easy to configure and use the App Service as compared to VM's.

VM would be a good solution when the following conditions would be met: 
- Legacy support is required.
- Complete control over the system is necessary.
- When we need to scale the app on the Ram Size i.e. more than 14 gb or increasing the cpu cores (4 Cores)

VM would be good option if we need any immediate modifications and changes in the environment. 
Also VM requires more time for maintence which actually is not required in the project.
If we can make this better by using azure then its great.