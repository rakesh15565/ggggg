pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main' , url:'https://github.com/rakesh15565/ggggg.git'
                        }
        }

        stage('Build') {
            steps {
                echo 'Building the project...'
                // Add your build commands here
            }
        }

        stage('Test') {
            steps {
                bat 'javac example.java'
                // Add your test commands here
            }
        }

        
    }

    post {
        always {
            echo 'Pipeline execution completed.'
        }
        success {
            echo 'Pipeline succeeded.'
        }
        failure {
            echo 'Pipeline failed.'
        }
    }
}