

node {
	stage ('GIT-SCM')
	{
	checkout scm
	}
	stage('Build')
	{
	sh 'mvn package'
	}
	stage('deploy')
	{
	sh 'docker ps'
	}
}
