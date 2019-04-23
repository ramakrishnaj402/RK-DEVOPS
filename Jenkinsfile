node
{
    stage('Git Checkout'){
	checkout scm 
    }
    stage('mvn'){

   sh 'mvn package'
   }
   stage('Build Docker Imager'){
   sh 'docker build -t depoly .'
   }
	stage('deploy'){
    sh 'docker run -dti --name cnt1 -p 8082:8080 deploy /bin/bash'   
    }
}
