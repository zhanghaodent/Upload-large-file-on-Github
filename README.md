# Upload-large-file-on-Github
Download the "git" and "git lfs"
git lfs install #Verify that the "git lfs" has installed successfully.
cd D:\XX #Specifying the URI path within the repository directory where the uploaded files are located.
git init
git lfs install
git lfs track * #tracking the uploaded files, * represents all files in the repository directory
git add .gitattributes
git remote add origin http://XXXXX.com #setup link between Github and local Github
git push origin master #upload the property files
git add * #adding the uploaded files, * represents all files in the repository
git commit -m "Git LFS commit" #添加大文件上传的说明
git push origin master #上传大文件

Bug and debug
Bug1: git push
fatal: The current branch master has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin master

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.
Debug1:git push --set-upstream origin master

Bug2:git push --set-upstream origin master
Everything up-to-date
branch 'master' set up to track 'origin/master'.
Debug2:git add .
git commit -m "message"
git push



