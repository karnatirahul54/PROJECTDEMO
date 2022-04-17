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
		
		
  		stage ('Build') {
   				git url: 'https://github.com/cyrille-leclerc/multi-module-maven-project'
   				 withMaven {
     						 sh "mvn clean verify"
   						 } // withMaven will discover the generated Maven artifacts, JUnit Surefire & FailSafe reports and FindBugs reports
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
