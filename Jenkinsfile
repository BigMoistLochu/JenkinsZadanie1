pipeline {
    agent any
    triggers {
    pollSCM('* * * * *')
}
    stage("Checkout") {
            steps {
                git url: 'https://github.com/BigMoistLochu/JenkinsZadanie1', branch: 'main'
            }
        }
    stages {
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

