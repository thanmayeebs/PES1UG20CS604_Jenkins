pipeline{
	agent any
	stages{
		stage('Build'){
			steps{
				sh 'g++ -c PES1UG20CS604.cpp'
				sh 'g-- -o PES1UG20CS604 PES1UG20CS604.cpp'
				echo 'build stage successful'
			}
		}
		
		stage('Test'){
			steps{
				sh './PES1UG20CS604'
				echo 'Test stage executed successfully'
			}
		}
		stage('Deploy'){
			steps{
				echo 'Deployed Successfully'
			}
		}
	}
	post{
		failure{
			echo 'Pipeline failed'
		}
	}
}
