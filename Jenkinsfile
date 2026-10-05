pipeline {

    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/samarthgarde/java-cicd-demo.git'
            }
        }

        stage('Build') {
            steps {
                bat 'mvn clean package'
            }
        }

        stage('Test') {
            steps {
                bat 'mvn test'
            }
        }

        stage('Deploy to Tomcat') {
            steps {
                bat '''
                    copy /Y "target\\java-cicd-demo.war" "C:\\Program Files\\Apache Software Foundation\\Tomcat 10.1\\webapps\\java-cicd-demo.war"
                '''
            }
        }

    }
}
