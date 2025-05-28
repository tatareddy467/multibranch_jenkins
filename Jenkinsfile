pipeline {
    agent any
    stages {
        stage ('Build') {
            steps {
                echo "Executing Multi branch pipeline from git"
            }
        }
        stage ('test') {
            steps {
                echo "Executing Test stage"
            }
        }
        stage ('deploytodev') {
            steps {
                echo "Executing dev deployment stage"
            }
        }
        stage ('deploytoprod') {
            steps {
                echo "Executing to prod deployment stage"
            }
        }
    }
}
