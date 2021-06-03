pipeline {
    // agent any
    node {
        env.NODEJS_HOME = "${tool 'Node 14.x'}"

        // on windows
        env.PATH="${env.NODEJS_HOME};${env.PATH}"
        sh 'npm --version'
    }
    // tools {
    //     nodejs "nodejs"
    // }
    stages {
        stage ('Start') {
            steps {
                echo "hello"
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
