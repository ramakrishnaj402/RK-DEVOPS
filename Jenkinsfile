node
{
stage('Git Checkout'){
	checkout scm   
    }
stage('Build'){
	sh 'mvn package'
	}
stage('Build Docker Imager'){
	sh 'cd /var/lib/jenkins/workspace/git-build-docker_deploy/gameoflife-web'
   	
    }
}
