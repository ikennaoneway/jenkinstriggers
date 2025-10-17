pipeline {
    agent any

    triggers {
        githubPush()   // Automatically triggers when you push code
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'git@github.com:<your-username>/jenkins-ci-demo.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building project...'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying project...'
            }
        }
    }
}
