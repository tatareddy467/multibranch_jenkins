pipeline {
    agent any
    environment {
        login = credentials('naani-user-jenkins-slave')
    }
    stages {
        stage ('Build') {
            steps {
                echo "login credentials are ${login}"
                echo "login user name is ${login_USR}"
                echo "login user password is ${login_PSW}"
            }
        }
    }
}
