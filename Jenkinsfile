pipeline {
  agent any
  stages {
    stage('COMPILE') {
      steps {
        sh 'mvn clean compile -DskipTests=true'
      }
    }

    stage('Build') {
      steps {
        sh 'mvn clean package -DskipTests=true'
      }
    }

    stage('publish') {
      steps {
        sh 'echo "completed successfully"'
      }
    }

  }
  tools {
    maven 'maven398'
  }
}