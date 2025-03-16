pipeline {
    agent any
    tools{
        maven  'maven398'
    }
    
    stages {
        stage('COMPILE') {
            steps {
                sh "mvn clean compile -DskipTests=true"
            }
        }
        
        stage('Build') {
            steps {
                sh "mvn clean package -DskipTests=true"
            }
        }        
        
    }
}
