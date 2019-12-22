pipeline {
    agent {
        docker { image 'maven' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'ls -l'
                sh 'touch aymantest'
            }
        }
    }
}
