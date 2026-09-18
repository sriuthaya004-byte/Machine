pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Pulling code from GitHub...'
            }
        }
        
        stage('Test Python') {
            steps {
                echo 'Running Python application...'
                sh 'python3 app.py' 
            }
        }

        stage('Compile Java') {
            steps {
                echo 'Compiling Java application...'
                sh 'javac app.java'
            }
        }
    }
}

