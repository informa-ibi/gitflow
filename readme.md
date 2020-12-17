Piched up new ticket from jira - P3-0002. Run git command
  **git flow feature start P3-0002**

Git creates new branch feature/P3-0002. You can work locally on this feature.
You have pusblish the feature before you finish it.
  **git flow feature publish P3-0002**
  
Now you nave to create the PR. 
**Notice: be sure that the PR has been compared with develop branch!!!**

When the PR is approved you have to finish feature
  **git flow feature finish P3-0002**
This command merge your feature branch into the develop.
Push the **develop** branch to remote
  **git push origin develop**
  

If we decided we are ready to release someone of developers have to start release    
  **git flow release start v1.02**
  
You have pusblish this release.  
  **git flow release publish v1.02**
Now you have to deploy this version to TEST environment.

Developes may fix issues during the validation but have to merge the changes to this release branch as usual.

When all defects\features validated you have to finish the release
  **git flow release finish v1.02**
  
Push the **master** branch to remote  
  **git push origin master**
 
Now you can to deploy this version to PROD environment. 