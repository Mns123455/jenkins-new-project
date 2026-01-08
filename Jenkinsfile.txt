pipeline {
    agent any
    stages {
        stage('Start') {
            steps {
                echo 'Starting new project build'
                bat 'mkdir output'
            }
        }
        stage('Build') {
            steps {
                bat 'echo Build task running > output/build.txt'
            }
        }
        stage('Finish') {
            steps {
                echo 'Build completed successfully'
            }
        }
    }
}
