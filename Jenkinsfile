pipeline {
    agent { label 'testslave' }
    stages {
        stage('Test Submodule') {
            steps {
                sh '''
                    cd ztp-lab
                    ls -l
                '''
            }
        }
    }
}
