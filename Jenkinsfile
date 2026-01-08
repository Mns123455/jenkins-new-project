pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat '''
                echo BUILD START
                mkdir output
                echo Build successful from Jenkins > output\\result.txt
                echo %DATE% %TIME%
                '''
            }
        }
    }
}
