pipeline {
    agent any
    tools {
        nodejs "nodejs"
    }
    stages {
        stage ('git') {
            steps {
                git 'https://github.com/4ward110/simple-ci'
            }
        }

        stage ('Build') {
            steps {
                sh 'npm install'
            }
        }

        stage ('Test') {
            steps {
                sh 'npm test'
            }
        }
    }
}
