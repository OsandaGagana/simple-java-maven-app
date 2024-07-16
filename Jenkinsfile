pipeline {
    agent any

    stages {
        stage('Build') {
            environment {
                PATH = "/opt/maven/bin:${env.PATH}"
            }
            steps {
                sh 'mvn -B -DskipTests clean package'
                //sh "echo ${env.PATH}"
                sh 'echo $PATH'
                //sh "echo ${env.HOME}"
                sh 'echo $HOME'
            }
        }
    }
}
