pipeline {
    agent any
    // This environment variables can be used accross all the stages
    environment {
        // key value pair
        name = "Naani"
        course = "k8s"
    } 
    stages {
        stage ('Build') {
            // This environment variable are specific to stage level only
            environment {
                cloud = "GCP"
                name = "Maha"
            }
            steps {
                echo "Welcome ${name}"
                echo "you enrolled to ${course} course"
                echo "you are certified in ${cloud}"
            }
        }
        stage ('secondstage') {
            steps {
                echo "Welcome ${name}"
                echo "you enrolled to ${course} course"
                echo "you are certified in ${cloud}"
            }
        }
    }
}
