pipeline {
    agent any
    tools {
        maven 'm1'
    }
    stages {
        stage('Build') {
           steps {
              echo "Cleaning the maven project"
              sh 'mvn clean'
           }
        }
        stage('Test') {
           steps {
              echo "Testing the Code"
              sh 'mvn package'
           }
        }
        stage('Deploy') {
           steps {
              echo "Deploying the Project"
           }
        }
    }
}
