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
    def dockerRun = 'docker run -dti --name cnt1 -p 8082:8080 deploy /bin/bash'   
    }
}
