pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                bat 'pip install -r requirements.txt'
            }
        }
        
        stage('Test') {
            steps {
                bat 'python -m pip install -r requirements.txt && python test.py'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'deployed'
            }
        }
    }
}
