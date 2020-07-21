# node-js-material

//Transfer our source  code to the third party server like (github,heroku,aws) in secure way by using SSH keys
//only share id_rsa.pub file not id_rsa it  is secret file 


SSH Key generateor cmd:  ssh-keygen -t rsa -b 4096 -C "amolw211@gmail.com"



//using gitbash run following cmd to start communcation securely with server

//search ssh file 
ls -a -l ~/.ssh

//enable ssh agent
 eval "$(ssh-agent -s)"
 
 //add secure prevate key
  ssh-add  ~/.ssh/id_rsa

//read content of you ssh file
cat ~/.ssh/id_rsa.pub

//test ssh connection
ssh -T git@github.com
