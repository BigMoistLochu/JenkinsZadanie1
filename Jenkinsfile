pipeline {
    agent any
    triggers {
    pollSCM('* * * * *')
}
    stages {
        stage("Checkout") {
            steps {
                git url: 'https://github.com/BigMoistLochu/JenkinsZadanie1/tree/main', branch: 'main'
            }
        }
        stage('Build') {
            steps {
                echo 'Building...'
                sh 'python3 calculator.py 3 3'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                sh 'python3 test_calculator.py'
            }
        }
    }
}

