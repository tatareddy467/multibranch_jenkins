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
                expression {
                    BRANCH_NAME ==~ /(production|staging)/
                }
            }
            steps {
                echo "Deploying to Stage environment"
            }
        }
    }
}
