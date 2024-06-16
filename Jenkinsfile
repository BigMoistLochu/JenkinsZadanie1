pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                python .\calculator.py 3 3
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                python .\test_calculator.py
            }
        }
    }
}
