pipeline {
    agent any
    
    tools {
        // Option 1-la neenga JDK-ku enna 'Name' kudutheengalo athai inge podanum
        jdk 'Java21' 
    }

    stages {
        stage('Checkout') {
            steps {
                echo 'Pulling code from GitHub...'
            }
        }
        
        stage('Check Java Version') {
            steps {
                // Java sariya update aagi irukka nu check panna
                sh 'java -version'
                sh 'javac -version'
            }
        }

        stage('Compile Java') {
            steps {
                echo 'Compiling Java application...'
                sh 'javac app.java'
            }
        }
        
        stage('Run Python') {
            steps {
                echo 'Running Python application...'
                sh 'python3 app.py' 
            }
        }
    }
}
