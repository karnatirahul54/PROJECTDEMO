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
                	sh 'mvn -B -DskipTests clean package'
            }
        }
        
        stage('Test') {
            steps {
                	sh 'mvn test'
            }
        }
   
		
		stage('Five') {
			steps {
				echo 'Finished'
			}
		}		
	}
}
