node{
    
    environment {
        CI = 'true' 
    }
    stage('Checkout'){
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'adb60ca1-1352-4c4f-8359-35111559643e', url: 'https://camiloduqued@bitbucket.org/camiloduqued/react-prod.git']]])
        echo PWD()
    }

    stage('Build') {
        sh 'npm install'
    }

    stage('Test') {
        echo "test"
    }

    stage('Deliver') {
        echo "deliver"
    }
}