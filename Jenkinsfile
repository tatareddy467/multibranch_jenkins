pipeline {
    agent any
    environment {
        DEPLOY_TO = 'production'
    }
    stages {
        stage ('Deploy'){
            when {
                equals expected: 'production', actual: "${DEPLOY_TO}"
                //equals expected: 5, actual: "${BUILD_NUMBER}" 
                //equals expected: 18, actual: "currentBuild.number"
                //environment name: 'DEPLOY_TO', value: 'production'

            }
            steps {
                echo "Deploying"
            }
        }
    }
}
