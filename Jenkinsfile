pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'I want to test'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'I am testing'
          }
        }

        stage('Deploy') {
          steps {
            echo 'Deployment'
          }
        }

      }
    }

  }
}