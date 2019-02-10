pipeline {
    agent any 
    stages {
        stage('clone repo and clean') { 
            steps {
                bat "mvn clean -f JavaHelloWorld"
            }
        }
        stage('Test') { 
            steps {
                bat "mvn test -f JavaHelloWorld" 
            }
        }
        stage('Deploy') { 
            steps {
                bat "mvn package -f JavaHelloWorld "
            }
        }
    }
}
