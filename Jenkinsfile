pipeline {

    agent {
        docker {
            image 'node:6-alpine'
            args '-p 3000:3000'
        }
    }

    stages {

        stage('Build') {

            steps {
                sh 'npm config set proxy http://10.10.5.18:8080'
                sh 'npm install'
            }
            
        }

    }

}
