To incorporate changes from the main branch into a feature branch, follow these steps:

1. **Update your local main branch**
    
    `git checkout main git pull origin main`
    
    This fetches the latest changes from the remote main branch.
    
2. **Switch to your feature branch**
    
    `git checkout feature-branch`
    
3. **Rebase the feature branch onto the main branch**
    `git rebase main`
    
    This moves your feature branch to start from the latest commit of the main branch, applying your changes on top of it.
    
4. **Resolve any conflicts** (if they arise) and continue rebasing:bash
    
    `git add <filename> git rebase --continue`
    
5. **Push your changes** (force push may be needed):
    
    `git push origin feature-branch --force`