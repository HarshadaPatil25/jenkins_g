pipeline {
	agent any
	stages{
		stage ('download from github') {
			steps {
				echo "downloadfromgithub"
				git ' https://github.com/vimallinuxworld13/simple-java-maven-app.git '
			}
		}	
		stage ( ' build ') {
			sh ' mvn clean package '
		}
 		stage ( 'deploy') {
			sh ' java -jar target/*.jar '
		}
	}
}