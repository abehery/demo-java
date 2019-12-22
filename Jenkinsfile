pipeline {
    agent {
        docker { image 'maven' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'ls -l'
                sh 'touch aymantest'
                def image = docker.build("chs/uaa-keycloak:latest", "--label UAA_VERSION=${uaa_version} --build-arg uaa_version=${uaa_version} .")
            }
        }
    }
}
