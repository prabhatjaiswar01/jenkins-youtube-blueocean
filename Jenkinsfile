pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''pwd
date'''
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test Step'
          }
        }

        stage('test parellel') {
          steps {
            echo 'test Parallel'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy'
        sleep 13
      }
    }

  }
}