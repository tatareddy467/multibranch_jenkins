pipeline {
    agent any 
    environment {
        name = "Naani"
        course = "K8S"
    }
    stages {
        stage ("Build") {
            steps {
                echo "Welcome ${name}"
                echo "You are enrolled to ${course}"
            }
        }
        stage ('Second Stage') {
            environment {
                name = "Pranav"
                cloud = "GCP"
            }
            steps {
                echo "Welcome to ${name}"
                echo "you are enrolled to ${course}"
                echo "you are certified in ${cloud}"
                sh "printenv"
            }
        }
    }
}
