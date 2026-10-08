
pipeline {
    agent any

<<<<<<< HEAD
    stages {
        stage('Checkout') {
            steps {
                echo 'Repository checkout successful'
            }
        }

        stage('Build') {
            steps {
                echo 'Build stage running'
=======
    environment {
        IMAGE_NAME = 'aslamnoushad22/devops-app'
        IMAGE_TAG = '1.0'
    }

    stages {
        stage('Checkout') {
            steps {
                echo 'Source code checked out by Jenkins SCM'
>>>>>>> 662b7f9 (Add Jenkins pipeline and multi-stage Dockerfile)
            }
        }

        stage('Test') {
            steps {
<<<<<<< HEAD
                echo 'Test stage running'
=======
                sh '''
                    docker build --target builder -t devops-app-test .
                    docker run --rm --entrypoint python \
                        devops-app-test -m pytest -v /build
                '''
            }
        }

        stage('Build Docker Image') {
            steps {
                sh '''
                    docker build -t ${IMAGE_NAME}:${IMAGE_TAG} .
                '''
>>>>>>> 662b7f9 (Add Jenkins pipeline and multi-stage Dockerfile)
            }
        }
    }

    post {
        success {
<<<<<<< HEAD
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed. Check the console output.'
=======
            echo 'Tests passed and Docker image built successfully.'
        }
        failure {
            echo 'Pipeline failed. Check the stage logs.'
>>>>>>> 662b7f9 (Add Jenkins pipeline and multi-stage Dockerfile)
        }
    }
}
