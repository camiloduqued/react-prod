pipeline {
    agent {
        docker {
            image 'node:6-alpine'
            args '-p 3000:3000'
        }
    }
    environment {
        CI = 'true'
    }
    stages {

        stage('Build') {
            steps {
                echo "build"
                //sh 'npm install'
            }
        }

        stage('Test') {
            steps {
                echo "tests3"
                //sh './scripts/test.sh'
            }
        }

        stage('Deliver') {
            steps {
                echo "deliver"
                //sh './scripts/deploy.sh'
                //input message: 'Finished using the web site? (Click "Proceed" to continue)'
                //sh './jenkins/scripts/kill.sh'
            }
        }

    }
}