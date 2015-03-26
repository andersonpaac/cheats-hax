#SSH Keys
ssh-keygen -t rsa -C ""

eval "$(ssh-agent -s)"

ssh-add ~/.ssh/id_rsa

ssh -T git@github.com

#VIM shortcuts
2w move two words forward
3b move two words backword
$ move to eol
0 move to behining of line
:set paste while copying indentation
:set nopaste after copying indentation
2< two unindent
3> 3 indents

#TMUX
" down
% up
n , p , x , c traverse

#PYTHON
Built in objects
1.	type(objectname)
2.  inspect- (package): inspect(objectname) will return all class members of object

#Markdown
** bold **
* italics *
~~ strikethrough~~
1.one
2.two
1.three but one
4.oho
-unordered here
+and here too
```python 
ok = 33
ok=ok+30
```
>Quotes here , length = infinity

#Git
git config --global user.name "anderson"
git config --global user.email ""
git config --global color.ui auto
git config --global alias.ci commit
git add *
git rm 
git commit -m ""
git push

git branch branchname
git checkout branchname
git pull origin branchname

After .gitignore file
git rm -r --cached .
git add .
git ci -m "Removed all unecessary files"

##For new repos
git remote add origin git@github.com:andersonpaac/cheats-hax.git

git push -u origin master

#Heroku
##One time setup
heroku login
heroku keys:add

##One time repo setup
heroku git:remote -a <APPNAME>

##Updating the repo
git push heroku master

##Heroku db migrate
 heroku run rake db:migrate

#Todo
grep
find
locate
regex
vimrc file
vim modules
sendgrid
