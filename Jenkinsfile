node
{
stage('Git Checkout'){
	checkout scm   
    }
stage('Build'){
	sh 'mvn package'
	}
stage('Build Docker Imager'){
   	sh 'docker build -t depoly .' {
   	 	sh 'docker run -dti --name cnt1 -p 8082:8080 deploy /bin/bash' 
	}
    }
}
