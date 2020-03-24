pipeline {
    agent { label 'testslave' }
    stages {
        stage('Test Submodule') {
            steps {
                sh '''
                    cd ztp-lab
                    git show-ref --head
                    ls -l
                    git checkout master
                    git show-ref --head
                    ls -l
                '''
            }
        }
        stage('Set env var') {
            steps {
                env.custom_var = "HELLO AIRBUS WORLD"
            }
        }
        stage('Test Env Var') {
            steps {
                echo "$env.custom_var"
            }
        }  
    }
}
