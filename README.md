# Git Workflow
Git, as a source code managing system, will inevitably come up with multi-people cooperation.  
Cooperation calls for a standard workflow to make others working effectively, keeping the project developing in good order.  
So what is the workflow? It will be introduced in this article.  
## Function driven development
Git workflow has an important feature: it applies **Featuren-driven development**  
That is to say, the demand is the start of the development. First comes demands, then comes the **feature branch** or **hotfix branch**.  
When the development is done, the branches are merged into the master branch, and are deleted afterwards.  
## Git flow
Git flow is the first and the most broadly used workflow.  
### Features
There are two main features of Git flow.  
Firstly, there are two long-term branches.
```
· master branch
· develop branch
```
The former deposits the version that is released. Whenever you get a version from the branch, it is always a stable version.  
Meanwhile, the latter is used for normal development, depositting the latest testing version.  
Secondly, there are three short-term branches.  
```
· feature branch  
· hotfix branch  
· release branch
```
Once the development is finished, they will be merged into **develop** or **master**, and is deleted afterwards.  
### Summary
The merit of Git flow is that it is clear and controllable. However, it is complex to some extent. Two long-term branches  
needs to be maintained in the same time.  
Most tools consider **master** as the default branch, however, since the development is done in the **develop** branch,   
which means developers need to shifting between the two branches frequently, wasting much energy.  
A bigger problem is that the mode is based on "version released", which aims to produce a new version in a period of time.  
But, a great many projects are "continously released", code is submitted once it is modified. Thus, there is little difference  
between **master** and **develop**. There is no need for maintaining the two long-term branches.
