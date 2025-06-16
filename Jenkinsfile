pipeline {
    agent any
    environment {
       Pranav = credentials ('naani-user-jenkins-slave')
    }
    stages {
        stage ('Build') {
            steps {
                echo "Git hub login credentials are ${Pranav}"
                echo "git hub user name is ${Pranav_USR}"
            }
        }
    }
}
