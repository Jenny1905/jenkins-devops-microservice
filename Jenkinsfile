pipeline{
	agent{ docker{ image 'maven:3.6.3'}}
	stages{
		stage('Build'){
			steps{
				//sh 'mvn --version'
				echo "Build"
				echo "$PATH"
				echp "BUILD_NUMBER - $env.BUILD_NUMBER"
				echo "BUILD_ID - $BUILD_ID"
 			}
		}
		stage('Test'){
			steps{
				echo "Test"
 			}
		}
		stage('Integration Test'){
			steps{
				echo "Integration Test"
			}
		}
	}
	post{
		always{
			echo 'Hurrah! Congratulations for running the stage!'
		}
		success{
			echo 'Stage successfully run...'
		}
		failure{
			echo 'stage failed'
		}
	}
	
}
