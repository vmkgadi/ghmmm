pipeline {
    agent any

    environment {
        APP_ENV = 'dev'
    }

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/vmkgadi/ghmmm.git'
            }
        }

        stage('Build') {
            steps {
                sh 'echo Building in $APP_ENV'
            }
        }

        stage('Test') {
            steps {
                sh 'echo Running tests'
            }
        }

        stage('Quality Gate') {
            steps {
                sh 'echo Checking Code'
                quality...'
            }
        }
    }
}
