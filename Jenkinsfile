pipeline {
    agent { label 'testslave' }
    stages {
        stage('Test Submodule') {
            steps {
                sh '''
                    cd ztp-lab
                    git show-ref --head
                    ls -l
                '''
            }
        }
    }
}
