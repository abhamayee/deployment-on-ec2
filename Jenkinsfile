pipeline {
  agent none
  stages {
    stage('Back-end') {
      agent {
        docker { image 'maven:3.8.1-openjdk-17' }
      }
      steps {
        sh 'mvn clean install'
        sh 'mvn spring-boot:run'
      }
    }
  }
}
