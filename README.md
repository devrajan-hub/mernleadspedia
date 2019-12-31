# mernleadspedia
LeadsPedia in MERN

# Install and Run Project
    npm install
    npm client-insall
    npm run dev

## GitHub Commands:
1.) First Time - Clone Single Branch: 
    <!-- directory address [/your/folder] is optional -->
    git clone https://github.com/rli46c/mernleadspedia.git -b alpha --single-branch /your/folder

2.) First Time - Update Config
    <!-- Add [--global] only if you want the same config for all repositories. -->
    git config --global user.email "you@example.com"
    git config --global user.name "Your Name"
    
3.) First Time - Link local Branch to Remote during first push
    <!-- Here "origin" is local branch name and "alpha" is remote branch name -->
### If you have not committed:
    git stash
    git checkout alpha
    git stash pop

### If you have committed and have not changed anything since:
    git log --oneline -n1 # this will give you the SHA
    git checkout alpha
    git merge ${commit-sha}

### If you have committed and then done extra work:
    git stash
    git log --oneline -n1 # this will give you the SHA
    git checkout alpha
    git merge ${commit-sha}
    git stash pop

    git push origin HEAD:alpha    

4.) Everytime - Add your changes and commit them
    <!-- Here . or all can be used to add all files. You can also add specific files/folders -->
    git add .
    git commit -m "Message"

5.) Everytime - Pull Further Changes: git pull
6.) Everytime - Push Further Changes: git push
