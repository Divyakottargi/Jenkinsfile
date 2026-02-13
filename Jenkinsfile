pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building the application...'
                bat 'echo "Version 1.0.5" > deploy_file.txt'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying to Jenkins Storage...'
                // This "Archives" the file so it appears on your dashboard
                archiveArtifacts artifacts: 'deploy_file.txt', fingerprint: true
            }
        }
    }
}
