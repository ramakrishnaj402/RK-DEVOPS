node
{
    stage('Git Checkout'){
	checkout scm 
    }
    stage('BUILD'){

   sh 'mvn package'
   }
   stage('Docker Imager & DEPLOY'){
   sh 'docker build -t depoly .'
   sh 'docker images'
   sh 'docker run -dti --name cnt1 -p 8082:8080 depoly /bin/bash'
   sh 'docker ps -a'
    }
}
