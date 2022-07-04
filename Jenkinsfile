pipeline {
	agent any
	stages{
		steps ('download from github') {
				echo "downloadfromgithub"
				git ' https://github.com/vimallinuxworld13/simple-java-maven-app.git '
			}
		}	
		steps( ' build ') {
			sh ' mvn clean package '
		}
 		steps ( 'deploy') {
			sh ' java -jar target/*.jar '
		}
	}
}