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
        sh 'mvn sonar:sonar -Dsonar.login=0df1838e9696187fce45ad96518fa40f61243254bae905e3113c968faa5636c6'
    }
}

    }
}
