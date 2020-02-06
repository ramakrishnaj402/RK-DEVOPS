node
{
    stage('Git Checkout'){
	checkout scm 
    }
    stage('BUILD'){

   sh 'mvn package'
   sh 'cp -b /var/lib/jenkins/workspace/git-build-docker_deploy/gameoflife-web/target/gameoflife.war /var/lib/jenkins/workspace/git-build-docker_deploy/target'
    }
   stage('Docker Imager & DEPLOY'){
   sh 'docker build -t depoly .'
   sh 'docker images'
   sh 'docker run -dti --name cnt5 -p 8082:8080 depoly /bin/bash'
   sh 'docker ps -a'
	 
    }
}
