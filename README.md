#SSH Keys

```
ssh-keygen -t rsa -C ""
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_rsa
```
#Linux


##Processes
```
ps aux #list all processes
kill << pid>> #kills pid without sudo
kill <<pid>> -9  #kills pid if previous doesnt' work
top #shows the processes taking the max amount of resources
```
###Searching
```
grep -R "<<search-term>>" <<path here>> #Searches the entire folder recursively for the search term

```
##Terminal
```
sudo scutil --set HostName <<hname>>#updates hostname in terminal
alias l=ls #Set l as ls
```
###just PS1 things
```
export PS1='\u@\h: ' #hides path
export PS1='> ' #super minimalistic only shows ">"
```
	
##VIM shortcuts
```
2w move two words forward
3b move two words backword
$ move to eol
0 move to behining of line
:set paste while copying indentation
:set nopaste after copying indentation
2< two unindent
3> 3 indents
o to create new line
#ctrl+- or cmd+- works to zoom on windows/mac
```
##TMUX
```
" down
% up
n , p , x , c traverse
```
#PYTHON
Built in objects
```Python
type(objectname)  #Built in 
inspect.getmembers(object) #will return all class members of object
```

#Markdown
```
** bold **
* italics *
~~ strikethrough~~
1.one
2.two
1.three but one
4.oho
-unordered here
+and here too
```
```python 
ok = 33
ok=ok+30
```
>Quotes here , length = infinity

#Git
```
git config --global user.name "anderson"
git config --global user.email ""
git config --global color.ui auto
git config --global alias.ci commit
ssh -T git@github.com
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
```
##For new repos
```
git remote add origin git@github.com:andersonpaac/cheats-hax.git
git push -u origin master
```
#Heroku
##One time setup
```
heroku login
heroku keys:add
```
##One time repo setup
```
heroku git:remote -a <APPNAME>
```
##Updating the repo
```
git push heroku master
```
##Heroku db migrate
```
heroku run rake db:migrate
```

#RPi
##DISABLE WIFI POWER MANAGEMENT
```
sudo nano /etc/modprobe.d/8192cu.conf
options 8192cu rtw_power_mgnt=0 rtw_enusbss=0
```
#Restart WIFI config from /etc/wpa_supplicant/wpa_supplicant.conf
wpa_cli reconfigure
wpa_cli status #status
#Fast nmap
```
nmap -sS -O 192.168.0.1-255 #OS detection + port scan
nmap -sn  192.168.1.100-140
```

#Postgres
```
	

```
