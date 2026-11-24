pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Run') {
            steps {
                sh 'python3 app.py'
            }
        }
        stage('Test') {
            steps {
                sh 'python3 -m unittest -v'
            }
        }
    }
}
