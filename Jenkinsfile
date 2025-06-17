pipeline {
    agent any 
    environment {
        DEPLOT_TO = 'production'
    }
    stages {
        stage ('Deploy') {
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
