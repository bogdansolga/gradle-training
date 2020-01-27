pipeline {
  agent {
    node {
      label 'the-most-powerful'
    }

  }
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'hello'
          }
        }

        stage('test') {
          steps {
            sleep 2
          }
        }

      }
    }

  }
}