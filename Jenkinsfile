pipeline {
    agent any
    environment {
        DEPLOY_TO = 'production'
    }
    stages {
        stage ('Deploy to') {
            when {
                environment name: 'DEPLOY_TO', value: 'production'
            }
            steps {
                echo "Deploying"
            }
        }
    }
}
