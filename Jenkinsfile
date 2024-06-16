pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                sh 'python calculator.py 3 3'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                sh 'python test_calculator.py'
            }
        }
    }
}

