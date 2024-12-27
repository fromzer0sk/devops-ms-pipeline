pipeline {
	agent {docker {image 'node:lts-jod'}}
	stages{
		stage('Build'){
			steps{
				 sh 'node --version' 
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
