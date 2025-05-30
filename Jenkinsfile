pipeline {
    agent any
    environment {
        name = "Naani"
        course = "K8S"
    }
    stages {
        stage ('Build') {
            steps {
                echo "Welcome ${name}"
                echo "You are enrolled ${course}"
            }
        }
        stage ('secondstage') {
            environment {
                cloud = "GCP"
                name = "vijaya"
            }
            steps {
                echo "Welcome ${name}"
                echo "You are enrolled ${course}"
                echo "you are certified in ${cloud}"
            }
        }
        stage ('thirdstage') {
            echo "Welcome ${name}"
            echo "You are enrolled ${course}"
            echo "you are certified in ${cloud}"
        }
    }
}
