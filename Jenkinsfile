pipeline {
    agent any
    stages {
        stage('CHECKOUT') {
            steps {
                script {
                    sh 'echo Checkout'
                    checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/mcieciorasii/aplikacja_kalkulator.git']]])
                }
            }
        } // END OF STAGE CHECKOUT
    }
}
