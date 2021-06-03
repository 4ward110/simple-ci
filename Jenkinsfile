pipeline {
    agent any
    tools {
        nodejs "node"
    }
    stages {
        stage ('git') {
            steps {
                git 'https://github.com/4ward110/simple-ci'
            }
        }

        stage ('Build') {
            steps {
                echo 'npm install'
            }
            sh 'npm install'
        }

        stage ('Test') {
            steps {
                sh 'npm test'
            }
        }
    }
}
