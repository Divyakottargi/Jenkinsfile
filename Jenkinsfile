pipeline {
    agent any
    stages {
        stage('GitHub Pull') {
            steps {
                echo 'Jenkins has successfully pulled the code from GitHub!'
            }
        }
        stage('Execution') {
            steps {
                bat 'echo Hello from GitHub Repo'
            }
        }
    }
}
