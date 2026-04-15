pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat 'sf --version'
            }
        }
        stage('Test') {
            steps {
                bat 'sf apex run test --test-level RunLocalTests --output-dir ./tests/apex --result-format tap'
            }
        }
    }
}
