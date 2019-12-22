pipeline {
    agent {
        docker { image 'slave-mvn-11' }
    }
    stages {
        stage('Test') {
            steps {
                script{
                sh 'ls -l'
                sh 'touch aymantest'
                def image = docker.build("chs/uaa-keycloak:latest", "--label UAA_VERSION=${uaa_version} --build-arg uaa_version=${uaa_version} .")
                }
            }
        }
    }
}
