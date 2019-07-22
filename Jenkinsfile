pipeline {
	agent any
	stages{
		stage('initial setup'){
			steps{
				sh 'echo starting'
			}
		}
		stage('Checking Docker'){
			steps{
				sh 'sudo docker ps'
			}
		}
		stage('starting build'){
			steps{
				sh 'sudo docker build --tag:php54 .'
			}
		}
	}
}
