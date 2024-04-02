//declrative
pipeline{
	agent any
	stages{
		stage('Build'){
			steps{
				echo "Build"
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
	}post{
		always{
			echo 'Hurrah! Congratulations for running the stage!'
		}
		success{
			'echo Stage successfully run...'
		}
		fail{
			'echo stage failed'
		}
	}
	
}
