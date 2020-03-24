pipeline {
  agent any
  stages {
    stage('Inicio') {
      steps {
        echo 'Wellcome'
        }
    }
    stage('Build') {
      steps {
        echo 'Wellcome test'
        sh 'docker build -t app .'
      }
    }
    stage('Test') {
      steps {
        echo 'Wellcome test'
      }
    }
    stage('Despliegue') {
      steps {
        echo 'Wellcome'
      }
    }

}
