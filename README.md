# EnterprisetoStdEdition
**SQLServer Enterprise Edition features detection: **

SQL Server Enterprise Edition provides datacenter capabilities with high performance, unlimited virtualization and many business intelligence tools. Sometimes it is not easy to identify if you are using any Enterprise Edition features or not.

This script will help you identify if you are using any Enterprise edition featuers or not. It covers the majority of use cases, however please be aware that it does not check each and every feature. 

**This script requires you to provide a login with view server state, view any database and connect any database. It will return a value of 1 if any of the below Enterprise Edition features are being used: **
1. Database level features 
2. Online Index Rebuild used outside DB Maintenance plan 
3. Read replicas of Availablity group
4. Asynchronous Replica of Availablity group 
5. Resource Governor 
6. R extention
7. Python extention
8. Memory Optimized tempdb metadata
9. more than 128G of memory 
10. more than 48 VCPU of CPU
11. Asynchronous mirroring

**Note: In order to find the Online index rebuild feature, you have to run the script during maintenance window during weekend or for minimum of a week on 5 min schedule basis so that you can capture all of the occurances. This script is very lightweight.

Please note that it is the customer's responsibility to determine if they are using any enterprise features.
