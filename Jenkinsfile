pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the project...'
                // Add build commands here, for example:
                // sh 'npm install'
                // sh './gradlew build' (for a Java project)
            }
        }
        stage('Test') {
            steps {
                echo 'Testing the project...'
                // Add test commands here, for example:
                // sh 'npm test'
                // sh './gradlew test' (for a Java project)
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the project...'
                // Add deploy commands here, for example:
                // sh 'scp target/your-app.jar user@server:/path/to/deploy'
            }
        }
        stage('Release') {
            steps {
                echo 'Releasing the project...'
                // Add release commands here, for example:
                // sh 'curl -X POST -H "Content-Type: application/json" -d \'{"tag_name": "v1.0.0", "name": "Release v1.0.0", "body": "Release description"}\' https://api.github.com/repos/your-repo/releases'
            }
        }
    }

    post {
        success {
            echo 'Pipeline succeeded!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}
