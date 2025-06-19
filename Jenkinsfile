pipeline {
    agent any
    stages {
        stage ('Build') {
            steps {
                echo "Welcome to Build stage"
            }
        }
        stage ('Deploy to Dev') {
            steps {
                echo "Deploying to Dev environment"
            }
        }
        stage ('Deploy to Stage') {
            when {
                branch 'production'
            }
            steps {
                echo "Deploying to Stage environment"
            }
        }
    }
}
