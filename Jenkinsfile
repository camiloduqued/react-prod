node{
    stage('Checkout'){
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'adb60ca1-1352-4c4f-8359-35111559643e', url: 'https://camiloduqued@bitbucket.org/camiloduqued/react-prod.git']]])
    }

    stage('Build') {
        echo "build"
    }

    stage('Test') {
        echo "test"
    }

    stage('Deliver') {
        echo "deliver"
    }
}