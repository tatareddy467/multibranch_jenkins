//This environment block can be used at pipeline level and stage level.
pipeline {
    agent any
    environment {
        // key value pair
        name = "Naani"
        course = "k8s"
    } 
    stages {
        stage ('Build') {
            steps {
                echo "Welcome ${name}"
                echo "you enrolled to ${course} course"
                //echo "you are certified in GCP"
            }
        }
    }
}
