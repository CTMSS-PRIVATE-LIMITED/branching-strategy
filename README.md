                      

GITHUB BRANCHING STRATEGY WORK FLOW :
 


*  Created a dummy organization in Github and Name of the Organization is CTMSS-PRIVATE-LIMITED.
* I Created a Repository and Repository Name is branching-strategy. Repository link 
 https://github.com/CTMSS-PRIVATE-LIMITED/branching-strategy .
* Created  below branches.
Main - This  main branch used for production releases. 
Dev - Once Developers ready with their code in the feature branches merged to Dev branch.
Feature- to develop new features that merged to the dev branch 
Release- help prepare a new production release; usually branched from the develop branch and must be merged back to both develop and main.
Hotfix- hotfix branches creates from a bug that has been discovered and must be resolved; it enables developers to keep working on their own changes on the develop branch while the bug is being fixed.


* Created below Teams in the repository.
1) Admin
2) Developer
3) Devops
4) QA
* Created below Members in the repository.
1) Praveen
2) Shashi
3) Satish
4) prvn20206

* Added Member Praveen  to Admin Team and provided the Admin permissions.
*Added Member Shashi to Developer Team and provided the Maintain permissions.
* Added Member Satish  to Devops Team and provided the Admin permissions.
* Added Member prvn20206 to QA Team and provided the Read permission.


* Started working on feature branch and Added below files.
src/main/webapp
target
Jenkinsfile
pom.xml
* After  adding above files into feature branch  in git . To push these files into feature branch in github by using below commands.
       git status
       git commit -am "GE-Vernova--dbr-updated pom.xml"
       git push origin feature

* Now i have raised a PR(Pull Request) for merge this code from feature branch to dev branch and  i have added branch protection rules like it is restrict to admins team and give permissions developers and devops teams and 1 member should need to review the code  and finally merge the code into dev branch by Developers team.

 

 

 

 





* Again i have  raised a PR(Pull Request) for merge this code from dev branch to release branch and  i have added branch protection rules like it is restrict to admins team and give permissions developers and devops teams and 1 member should need to review the code and finally merge the code into release branch by Developers team.

 

 

 

 

 





* Again raised a PR(Pull Request) for merge this code from release branch to main branch and  and  i have added branch protection rules like it is restrict to admins and developers Teams give permissions to devops teams and 1 member should need to review the code and finally merge the code into main branch by Deveops team.

 

 

 


 



 

*If we found any bugs in production  we create a hotfix branch and work on bugs. Once bugs are resolved merge this code to main branch and dev branch.

        







