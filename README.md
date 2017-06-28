For educational purposes only
=

Please note that this project contains some very obvious antipatterns 
and perhaps some not so obvious bad practices. 
For example, the database and the database passwords are deliberately 
  left in the project to show the reader how I have set up my development 
  environment. 
  
I've set up a bash alias in ~/.bash_alias. Something to the effect of: 

    cd /home/panda/Documents/src/mydrupal/;
    git add .;
    git commit -sS;
    git pull origin master;
    rsync -av /home/panda/Documents/src/mydrupal/SiteOne/ /var/www/html/;
    git push origin master;

This should update your site on localhost with your latest changes. 