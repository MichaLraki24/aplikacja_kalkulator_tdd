pipeline {
    agent any
    parameters {
        gitParameter branchFilter: 'origin/(.*)', defaultValue: 'main', name: 'BRANCH', type: 'PT_BRANCH'
    }
    stages {
        stage('CHECKOUT') {
            steps {
                script {
                    sh 'echo branch: ${params.BRANCH}'
                    checkout([$class: 'GitSCM', branches: [[name: '${params.BRANCH}']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/MichaLraki24/aplikacja_kalkulator_tdd.git']]])
                }
            }
        } // END OF STAGE CHECKOUT
    }
}
