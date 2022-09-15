pipeline {
agent {
label 'Build-Server'
}

stages {

stage ('Checkout') 
{
steps
    {
    
        checkout scm
        
    }
    
}
stage ('Build') 
{
    steps
    {
       sh "cd /home/ubuntu/workspace/frontend ; sudo npm install " 
    }
}

   
stage ('Deployment')
    {
    steps
    {
        sh "cd /home/ubuntu/workspace/frontend; sudo pm2 start app.js  " 
    }
}
  

}
}
    
    
