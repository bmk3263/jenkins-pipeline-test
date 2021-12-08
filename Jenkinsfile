pipeline {
    agent {
        docker {
                      
            image 'node:14-alpine'
            label 'docker-master'
        }
    }
    stages {
        stage('Test') {
            steps {
                sh 'node --version'
            }
        }
    }
}
