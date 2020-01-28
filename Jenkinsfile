pipeline {
  agent any
  
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

    stage('sequential-edited') {
      parallel {
        stage('sequential-edited') {
          steps {
            echo 'sequential'
          }
        }

        stage('another-stage') {
          steps {
            sleep 1
          }
        }

      }
    }

  }
}
