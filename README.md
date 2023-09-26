# EnterprisetoStdEdition
**SQLServer Enterprise Edition features detection: **

SQL Server Enterprise Edition provides datacenter capabilities with high performance, unlimited virtualization and many business intelligence tools. Sometimes it is not easy to identify if you are using any Enterprise Edition features or not.

This script will help you identify if you are using any Enterprise edition featuers or not, it cover majority of use case, it does not check each and every feature, but covers the most commonly used features. 

**This script requires you to provide login with view server state,view any database and connect any database. It will retun 1 if any of the bellow Enterprise Edition features are being used. **
It checks following features:
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

**Note: Online index rebuild feature is commonly used Enterprise level feature, Please check your index jobs if you are using rebuild online index or not.

Please note that it is the customers responsibility to make sure you are not using any enterprise features or not.
