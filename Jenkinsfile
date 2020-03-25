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
        sh '''
        docker stop web
        docer rm web
        docker run -itd -p 80:80 --name web --rm app'
        '''
      }
    }
    stage('Despliegue') {
      steps {
        echo 'Wellcome'
      }
    }
}
}
