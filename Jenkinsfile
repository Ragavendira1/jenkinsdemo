pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'building'
      }
    }

    stage('Test Firefox') {
      parallel {
        stage('Test Firefox') {
          steps {
            sh '''echo "Testing firefox"
'''
          }
        }

        stage('Test chrome') {
          steps {
            sh 'echo "Test Chrome"'
          }
        }

        stage('Test Edge') {
          steps {
            sh 'echo "Test Edge"'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy'
      }
    }

  }
}