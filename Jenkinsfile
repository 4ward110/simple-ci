pipeline {
    agent any
    node {
        env.NODEJS_HOME = "${tool 'Node 6.x'}"

        env.PATH="${env.NODEJS_HOME};${env.PATH}"
        sh 'npm --version'
    }
    stages {
        stage ('setup') {
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
