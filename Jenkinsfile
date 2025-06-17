pipeline {
    agent any 
    environment {
        DEPLOY_TO = 'production'
    }
    stages {
        stage ('Deployment stage') {
            when {
                //environment name: 'DEPLOY_TO', value: 'production'
                equals expected: 'production', actual: "${DEPLOY_TO}"
            }
            steps {
                echo "Deploying"
            }
        }
    }
}
