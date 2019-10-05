pipeline {
    agent any

    stages {
        stage ('clean') {
            steps {
                withMaven(maven : 'Maven 3.6.2') {
                    sh 'mvn clean'
                }
            }
        }
        stage ('verify') {
            steps {
                withMaven(maven : 'Maven 3.6.2') {
                    sh 'mvn verify'
                }
            }
        }
    }
}