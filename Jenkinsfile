pipeline {
    agent any

    tools {
        jdk 'JDK25'
    }

    stages {
        stage('Compile') {
            steps {
                bat 'javac Hello.java'
            }
        }

        stage('Run') {
            steps {
                bat 'java Hello'
            }
        }

        stage('Archive') {
            steps {
                archiveArtifacts artifacts: '*.class'
            }
        }
    }
}
