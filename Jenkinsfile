pipeline {
    agent any
    parameters {
        gitParameter branchFilter: 'origin/(.*)', defaultValue: 'main', name: 'BRANCH', type: 'PT_BRANCH'
        choice(name: 'TESTING LEVEL', choices: ['smoke', 'regression', 'nightly'], description: '')
    }
    stages {
        stage('CHECKOUT') {
            steps {
                script {
                    sh 'echo branch: ${BRANCH}'
                    checkout([$class: 'GitSCM', branches: [[name: '${BRANCH}']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/MichaLraki24/aplikacja_kalkulator_tdd.git']]])
                }
            }
        } // END OF STAGE CHECKOUT
        stage('TESTING') {
            steps {
                script {
                    sh 'echo branch: ${TESTING LEVEL}'
                }
            }
        } // END OF STAGE TESTING
    }
}
