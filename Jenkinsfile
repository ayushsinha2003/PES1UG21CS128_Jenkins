pipeline{
	agent any
	stages{
		stage('Build'){
			steps{
				build 'PES1UG21CS128-1'
				sh 'g++ main.cpp -o output'
			}
		}
		stage('Test'){
			steps{
				sh './outhgfhfput'
			}
		}
		stage('Deploy'){
			steps{
				echo 'deploy'
			}
		}
	}
	post{
		failure{
			error 'Pipeline failed'
		}
	}
}
