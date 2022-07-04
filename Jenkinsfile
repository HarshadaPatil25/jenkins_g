pipeline {
	agent any
	stages{
		stage('download from github') {
			    steps	echo "downloadfromgithub"
				git ' https://github.com/vimallinuxworld13/simple-java-maven-app.git '
			}	
		stage( ' build ') {
			    steps sh ' mvn clean package '
		}
 		stage( 'deploy') {
			    steps sh ' java -jar target/*.jar '
		}
	}
}