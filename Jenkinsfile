pipeline {
    agent any

    tools {
        // Define Maven tool by name and version configured in Jenkins
        maven 'Maven'
    }

    stages {
        stage('Checkout') {
            steps {
                // Checkout your source code from version control
                git branch: 'main', url: 'https://github.com/ravibiradar1985/For-GIT.git'
            }
        }

        stage('Build') {
            steps {
                // Use configured Maven tool to build the project
                sh 'mvn clean package'
            }
        }
    }
}
