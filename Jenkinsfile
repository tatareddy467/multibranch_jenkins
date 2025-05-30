// when condition should have atleast one condition
// https://www.jenkins.io/doc/book/pipeline/syntax/#when
pipeline {
    agent any
    environment {
        DEPLOY_TO = 'production'
    }
    stages {
        stage ('Deploy'){
            when {
                environment name: 'DEPLOY_TO', value: 'production'

            }
            steps {
                echo "Deploying"
            }
        }
    }
}
