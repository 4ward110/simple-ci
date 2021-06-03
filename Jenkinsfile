pipeline {
    agent any

    stages {
        stage ('setup') {
            steps {
                echo "hello world"
                
            }
        }
        stage ('build') {
            steps {
                sh 'npm install'
            }
        }
        stage ('test') {
            steps {
                sh 'mocha test'
            }
        }
    }
}