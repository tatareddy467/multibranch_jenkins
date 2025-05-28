pipeline {
    agent any
    tools {
        maven 'My_Maven'
    }
    stages {
        stage ('Maven') {
            steps {
                echo "Welcome to tools example"
                sh "mvn --version"
            }
        }
        stage ('other maven') {
            tools {
                jdk 'jdk_17'
            }
            steps {
                echo "Maven version with jdk 17"
                sh "mvn --version"
            }
        }
    }
}
