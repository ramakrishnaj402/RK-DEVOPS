

node {
	stage ('GIT-SCM')
	{
	checkout scm
	}
	stage('Build')
	{
	sh 'mvn package'
	}

}
