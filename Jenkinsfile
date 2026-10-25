pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Source code checkout'
            }
        }

        stage('Test') {
            steps {
                sh 'python3 -m unittest -v'
            }
        }

        stage('Package') {
            steps {
                sh 'python3 setup.py sdist'
            }
        }
    }
}