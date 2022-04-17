pipeline {
	agent any
	stages {
		stage('One') {
			steps {
				echo 'Hi, this is Soumitra from roytuts'
			}
		}
		
		stage('Two') {
			steps {
				input('Do you want to proceed?')
			}
		}
		
		stage('Build') {
            steps {
                	gradlew build
            }
        }
        
        stage('Test') {
            steps {
                	gradlew test
            }
        }
        
        stage('Check') {
            steps {
             		gradlew check
            }
        }      
		
		stage('Five') {
			steps {
				echo 'Finished'
			}
		}		
	}
}
