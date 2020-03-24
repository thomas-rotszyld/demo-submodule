pipeline {
    agent { label 'testslave' }
    stages {
        stage('Test Submodule') {
            steps {
                sh '''
                    cd ztp-lab
                    git checkout master
                    ls -l
                '''
            }
        }
    }
}
