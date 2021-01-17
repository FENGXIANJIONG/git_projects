Jan 16th

push files to github:

#http://www.testclass.net/git/git-commit-code/
#
git init
git add file name
git add .
git commit -m 'comments'
git remote add origin git@github.com:xxxxx/project_name.git
git push -u orign master

#########################
Attn.
1,project_name 
2,config settings
git config --global user.name ""
git config --global user.email ""
git init
git status
 
3,permission denied(publickey)
solutions
create publickey:
ssh-keygen -t rsa -C "email add"
ssh -v git@github.com
ssh-agent -s
ssh-add ~/.ssh/id_rsa

##server config:
copy id_rsa.pub to github->settings->SSH Keys->New key

git log
git reset --hard HEAD^//HEAD~1

##![reject] failed to push some ref....
git pull
