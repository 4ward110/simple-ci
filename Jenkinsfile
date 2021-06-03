pipeline {
    agent any
    tools {nodejs "nodejs"}
    stages {
        stage ('setup') {
            steps {
                echo "hello world"
                
            }
        }
        stage ('build') {
            steps {
                echo 'npm install'
            }
            sh 'npm install'
        }
        stage ('test') {
            steps {
                echo 'npm test'
            }
        }
    }
}
