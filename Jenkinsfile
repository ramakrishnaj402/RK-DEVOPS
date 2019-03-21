

node {
	stage ('GIT')
	{
	checkout scm
	}
	stage('Build')
	{
	sh 'mvn package'
	}

}
