pipeline {
  agent any
  stages {
    stage('Maven in docker') {
        agent { docker 'maven:3.3.9-jdk-8-alpine' }
        steps {
            sh 'mvn -v'
        }
    }
}
}
