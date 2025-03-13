@Library('my-shared-library') _ 

pipeline {
    agent any

    stages {
        stage('Initialize') {
            steps {
                script {
                    echo "Initializing the pipeline"
                    exampleStep()  // Calling the shared library step
                }
            }
        }

        stage('Build') {
            steps {
                script {
                    echo 'Building the application...'
                    exampleStep() // Ensure this function exists in your shared library
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
