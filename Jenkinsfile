pipeline {
    agent any 
    stages {
        stage ('Build') {
            steps {
                echo "Welcome to Build Stage"
            }
        }
        stage ('Deploy to Dev') {
            steps {
                echo "deploying to Dev environment"
            }
        }
        stage ('Deploy to Stage') {
            when {
                expression {
                    // stage should execute with either production branch or staging branch
                    BRANCH_NAME ==~ /(production|staging)/
                }
            }
            steps {
                echo "deploying to stage environment"
            }
        }
    }
}
