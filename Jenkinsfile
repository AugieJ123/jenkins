pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building the project'
      }
    }

    stage('Testing') {
      parallel {
        stage('Testing') {
          steps {
            echo 'Testing phase'
          }
        }

        stage('Testing 2') {
          steps {
            echo 'Phase 2 of the testing'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying to git hub'
      }
    }

  }
}