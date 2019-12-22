pipeline {
    agent {
        docker { 
            image 'slave-mvn-11'
            args '-u root -v /var/run/docker.sock:/var/run/docker.sock'
        }
        
    }
    stages {
        stage('Test') {
            steps {
                script{
                sh 'ls -l'
                sh 'touch aymantest'
                def image = docker.build("chs/uaa-keycloak:latest")
                }
            }
        }
    }
}
