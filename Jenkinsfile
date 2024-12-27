pipeline {
	//agent {docker {image 'node:lts-jod'}}
	agent any
	environment{
		dockerHome = tool "MyDocker"
		mavenHome = tool "myMaven"
		PATH = "$dockerHome/bin:$mavenHome/bin:$PATH"
	}
	stages{
		stage('Build'){
			steps{
				 //sh 'node --version'
				 sh 'mvn --version'
				 sh 'docker version' 
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
