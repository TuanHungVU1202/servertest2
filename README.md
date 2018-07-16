# serverTest2 - WORKING
#Update last time for serverTest2, continue to testStreamCam2
#PUSH TO ORIGIN MASTER
# To update gitHub everytime code changes
  1. git add .
  2. git commit -m "updates done by..."  // Remember to commit everytime it changes to see the different.
  3. git push origin <repo_name>
  
#To initial a new dir, see https://help.github.com/articles/adding-an-existing-project-to-github-using-the-command-line/
 
#If in anycase that not work, use
  git remote rm origin
  
  to remove origin instead of using another dir like "github, github1" and so on.
  
# To update VM
  1. Delete directory and its contents by (while at root dir)
    sudo rm [servertest2] -r
  2. sudo git clone [link]
  3. cd to new dir and run app the same way with running app on local machine 
      <code>node index.js</code>
  
# To access server after deployment
http://35.240.227.109:8000 (WITHOUT "s" in "http")


# For MongoDB
  1. Access https://mlab.com/home; Creat Users with Password.
  2. Use link mongodb://<dbuser>:<dbpassword>@ds139942.mlab.com:39942/mongotest-1 (link should change because of the diffirent accounts)
  
  Notes: install mongoDB ver 2.2.33 only to use <function(err,db)> with <db.collection> and so on.
  #Use 
  <code>npm uninstall mongodb --save

        npm install mongodb@2.2.33 --save</code>

  See package.json for more details


#Remember to pull if made any change remotely.

#This folder for establishing server only.

#Camera streaming not working, will update later.
