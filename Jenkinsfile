pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''pwd
date'''
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'code test'
          }
        }

        stage('test paralle') {
          steps {
            echo 'test par'
          }
        }

      }
    }

    stage('deploy test') {
      steps {
        echo 'deploy to test'
      }
    }

  }
}