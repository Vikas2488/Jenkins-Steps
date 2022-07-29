pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''pwd
date'''
      }
    }

    stage('print') {
      parallel {
        stage('print') {
          steps {
            echo 'test step'
          }
        }

        stage('print par') {
          steps {
            echo 'print vikas'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploy on production'
        sleep 3
      }
    }

  }
}