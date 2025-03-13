@Library('my-shared-library') _

pipeline {
    agent any

    stages {
        stage('Initialize') {
            steps {
                script {
                    echo "Initializing the pipeline"
                    exampleStep()  // Calling function from Shared Library
                }
            }
            
            stage('Build') {
                steps {
                    script {
                        echo 'Building the application...'
                        exampleStep() // Using function from shared library
                    }
                }
            }

            stage('Test') {
                steps {
                    script {
                        echo 'Running tests...'
                        exampleStep()
                    }
                }
            }

            stage('Deploy') {
                steps {
                    script {
                        exampleStep() // Using the shared function again
                        echo 'Deploying the application...'
                    }
                }
            }
        }
}
}
