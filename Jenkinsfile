pipeline {
    agent any
    environment {
        DEPLOY_TO = 'production'
    }
    stages {
        stage ('Build') {
            steps {
                echo "Welcome to build stage"
            }
        }
        stage ('Deploy to Dev') {
            steps {
                echo "Deploying to Dev environment"
            }
        }
        stage ('Deploy to Stage') {
            when {
                anyOf {
                    branch 'production'
                    environment name: 'DEPLOY_TO', value: 'productions' // this condition should fail but stage should execure bcoz of anyOf condition
                }
            }
            steps {
                echo "Deploying to Stage environment"
            }
        }
    }
}
