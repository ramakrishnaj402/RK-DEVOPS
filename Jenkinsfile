node
{
	stage('Git Checkout'){
		checkout scm   
		}
	stage('Build'){
	sh 'mvn package'
	}
stage('Build Docker Imager'){
	docker images
	}

   	
    }
