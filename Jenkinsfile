pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout source code from GitHub
                checkout([$class: 'GitSCM', branches: [[name: '*/main']], userRemoteConfigs: [[url: 'https://github.com/2100030263/ALM.git']]])
            }
        }

        stage('Run') {
            steps {
                // Run your Java application
                bat 'javac Karthik.java' // Replace with your actual Java file name
                bat 'java Karthik'

                bat 'python Karthik.py' // Replace with your actual Java file name
            
            }
        }
    }
}
