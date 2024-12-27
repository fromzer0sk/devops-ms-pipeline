pipeline {
	agent {docker {image 'maven:3.6.3'}}
	stages{
		stage('Build'){
			steps{
				 sh 'mvn --version' 
				 echo "Build"
			}
		}
		stage('Test'){
			steps{
				 echo "Testing"
			}
		}
		stage('Intigration Testing'){
			steps{
				 echo "Intigrating"
			}
		}
	}

	post{
		always{
			echo "I run always"

		}
		success{
            echo "I run when success"
		}
		failure{
			echo "I run when failure"

		}
	}
	
}
