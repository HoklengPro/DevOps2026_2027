pipeline {
    agent any

    stages {
        stage('Compile') {
            steps {
                sh 'mkdir -p bin'
                sh 'javac -d bin src/Main.java'
            }
        }
        stage('Run') {
            steps {
                sh 'java -cp bin Main'
            }
        }
    }
}
