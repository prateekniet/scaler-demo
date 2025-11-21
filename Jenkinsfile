pipeline {
    agent { label 'agent-1'
          }
    stages {
        stage('Parallel Work') {
            parallel {
                stage('Unit Tests') {
                    steps {
                        echo "Running unit tests..."
                        sh 'sleep 3'
                    }
                }
                stage('Integration Tests') {
                    steps {
                        echo "Running integration tests..."
                        sh 'sleep 5'
                    }
                }
                stage('Security Scan') {
                    steps {
                        echo "Running security scan..."
                        sh 'sleep 4'
                    }
                }
            }
        }
    }
}
