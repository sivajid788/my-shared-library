@Library('my-shared-library') _

pipeline {
    agent any

    stages {
        stage('Initialize') {
            steps {
                script {
                    echo "Initializing the pipeline"
                    exampleStep()  // Make sure this function exists in your shared library
                }
            }
        }
        
        stage('Build') {
            steps {
                script {
                    echo 'Building...'
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    echo 'Running Tests...'
                }
            }
        }
        
        stage('Deploy') {
            steps {
                script {
                    exampleStep()
                    echo 'Deploying application...'
                }
            }
        }
    }
} 
