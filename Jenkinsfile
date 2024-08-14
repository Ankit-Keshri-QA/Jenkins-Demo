node {
    try {
        stage('Build') {
            echo 'Building...'
            // Example: sh 'mvn clean install'
        }

        stage('Test') {
            echo 'Testing...'
            // Example: sh 'mvn test'
        }

        stage('Deploy') {
            echo 'Deploying...'
            // Example: sh 'scp target/*.jar user@server:/path/to/deploy'
        }
    } catch (Exception e) {
        currentBuild.result = 'FAILURE'
        echo 'Pipeline failed!'
        throw e
    } finally {
        echo 'Pipeline completed.'
    }
}
