pipeline {
    agent any

    stages {
        stage('checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/haiderrzaidi/MLops_Script.git'
            }
        }
        
        stage('Build') {
            steps {
                echo 'Building'
                bat 'pip3 install -r requirements.txt'
            }
        }
        
        stage('Test') {
            steps {
                echo 'Test'
                bat 'python test.py'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploy'
            }
        }
    }
}
