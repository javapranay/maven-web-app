pipeline {  
    agent any
    tools{
        maven "maven-3.9.9"
    }
    stages {
        stage('Git Clone') {
            steps {
               git 'https://github.com/javapranay/maven-web-app.git'
            }
        }
        stage('Maven Build') {
            steps {
               sh 'mvn clean package'
            }
        }
    }
}
