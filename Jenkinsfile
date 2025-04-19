pipeline {
    agent any
    
    tools {
        maven 'Maven 3.6.3'
    }

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/AmitPrajapati9401/jenkinsjavacoderepo.git'  // Replace with actual repo
            }
        }

        stage('Build') {
            steps {
                dir('my-app') {  // Change to actual repo folder
                    bat 'mvn clean package'
                }
            }
        }
    }

    post {
        always {
            echo 'Pipeline execution completed!'
        }
    }
}
