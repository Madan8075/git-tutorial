pipeline {
    agent any

    stages {
        stage('Develop') {
            steps {
                echo 'Hello World Develop stage'
            }
        }
        stage('Build') {
            steps {
                echo 'Hello Madan Build stage'
            }
        }
        stage('Test') {
            steps {
                echo 'Hello Madan Test'
                emailext body: '''Hello,checking the pipeline job''', subject: 'from jenkins', to: 'info@kshetravihari.com'
            }
        }
    }
}
