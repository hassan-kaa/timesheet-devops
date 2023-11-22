pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('GIT') {
            steps {
                echo 'Getting project from Git';
            }
        }
        stage('MAVEN CLEAN') {
            steps {
               sh 'mvn clean install'
            }
        }
        stage('MAVEN COMPILE') {
            steps {
                sh 'mvn compile'
            }
        }
        stage('MAVEN SONARQUBE') {
    steps {
        sh 'mvn sonar:sonar -Dsonar.login=squ_d80d1aac6eaaa55ca4b2fb8a745634f05905bbb6'
    }
}

    }
}
