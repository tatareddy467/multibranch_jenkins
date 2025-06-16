pipeline {
    agent any
    environment {
        name = "Naani"
        course = "K8S"
    }
    stages {
        stage ('Build') {
            environment {
                cloud = "GCP"
            }
            steps {
                echo "Welcome ${name}"
                echo "you are enrolled to ${course}"
                echo "you are certified in ${cloud}"
            }
        }
        stage ('Second Stage') {
            steps {
                echo "Welcome ${name}"
                echo "you are enrolled to ${course}"
                echo "you are certified in ${cloud}"                
            }
        }
    }
}
