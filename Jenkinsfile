pipeline {
	agent any
	stages{
		stage('download from github') {
			    steps	{ echo "downloadfromgithub"
				  git credentialsId: '33c5d30d-2ed7-4fb6-8cc0-a23df882c8d2', url: 								 'https://github.com/vimallinuxworld13/simple-java-maven-app.git'
			}
		}
		stage( ' build ') {
			    steps { sh 'mvn clean package'
			   }
 		 }
		stage( 'deploy') {
			    steps { sh ' java -jar target/*.jar '
			   }
		}
	}
}