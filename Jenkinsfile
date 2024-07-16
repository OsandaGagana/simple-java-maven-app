
pipeline {
    agent any
    tools {
        maven 'Maven 3.9.4' // Name of the Maven installation configured in Jenkins
    }
    stages {
        stage('Print Environment Variables') {
            steps {
                sh 'printenv'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn -B -DskipTests clean package'
            }
        }
    }
}
