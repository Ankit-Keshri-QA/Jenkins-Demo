pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                // Example: sh 'mvn clean install' (for Maven build)
            }
        }
        
        stage('Test') {
            steps {
                echo 'Testing...'
                // Example: sh 'mvn test' (for running tests)
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Example: sh 'scp target/*.jar user@server:/path/to/deploy' (for deploying)
            }
        }
    }
    
    post {
        always {
            echo 'Pipeline completed.'
        }
        
        success {
            echo 'Pipeline succeeded!'
        }
        
        failure {
            echo 'Pipeline failed!'
        }
    }
}
