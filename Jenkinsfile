pipeline{
	agent any
	
	stages{
		stage('Complie stage'){
		
			steps{
				withMaven(maven:'M3'){
					sh 'mvn clean complie'
				}
			}
		}
		
		stage('Testing stage'){
		
			steps{
				withMaven(maven:'M3'){
					sh 'mvn test'
				}
			}
		}
		
		stage('Deploy stage'){
		
			steps{
				withMaven(maven:'M3'){
					sh 'mvn deploy'
				}
			}
		}
	}
}
