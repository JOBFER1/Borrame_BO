pipeline {
  agent any
  stages {
    stage('Source') {
      steps {
        git 'https://github.com/JOBFER1/Borrame_BO.git'
      }
    }

    stage('Build') {
      steps {
        tool 'MAVEN_3_8_6'
        bat 'mvn clean package'
      }
    }

  }
  environment {
    COMPLETED_MSG = 'Hola!!!'
  }
}