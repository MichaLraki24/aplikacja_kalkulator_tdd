pipeline {
    agent any
    stages {
        stage('CHECKOUT') {
            steps {
                script {
                    sh 'echo branch: $BRANCH'
                    sh 'echo ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^'
                    sh 'echo git branch -r'
                    sh 'echo ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^'
                    
                    
                    
                    //input 'BRANCH'
                    //checkout([$class: 'GitSCM', branches: [[name: '$BRANCH']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/MichaLraki24/aplikacja_kalkulator_tdd.git']]])
                }
            }
        } // END OF STAGE CHECKOUT
    }
}
