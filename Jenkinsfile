pipeline {
    agent any
    environment {
        // credentials ('id'), this id should be the same from jenkins credentials
        Slave_Login = credentials ('naani-user-jenkins-slave')
        name = "NAANI"
    }
    stages {
        stage ('Build') {
            steps {
                echo "Slave login credentials are ${Slave_Login}"
                echo "slave login user name is ${Slave_Login_USR}"
                echo "slave login password is ${Slave_Login_PWD}"
            }
        }
    }
}
