pipeline {
	agent { label 'jdk8' }
	stages {
		stage('SourceCode')
	{
		steps {
		git url: 'https://github.com/aulapathisaikiran/spring-petclinic.git',branch: 'main'
}
	}
		stage('build the code')
{
		steps{
		sh script: 'mvn clean package'
}
}
		stage('Reporting the Archiving') {
		steps {
		junit testResults: 'target/surefire-reports/*.xml'			
}
}
}
}
