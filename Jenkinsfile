pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Build') {
            steps {
                echo 'Hello Madan Build'
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
