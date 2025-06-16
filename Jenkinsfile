pipeline {
    agent any
    environment {
        Jenkins_Creds = credentials ('testingforjenkinscredentials')
        name = "test"
    }
    stages {
        stage ('Build') {
            steps {
                echo "login credentials are ${Jenkins_Creds}"
                echo "login user name is ${Jenkins_Creds_USR}"
                echo "login user password is ${Jenkins_Creds_PSW}"
            }
        }
    }
}
