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
				sh 'sudo docker build --tag=php54 .'
			}
		}
		stage('starting docker-compose'){
			steps{
				sh 'sudo docker-compose up -d'
			}
		}
	}
}
