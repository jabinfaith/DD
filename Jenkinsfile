pipeline {
  agent none
  stages {
    stage('Build') {
      steps {
        echo 'Pull the build from GIT'
        echo 'Create a build using repo'
        echo 'Create a build using repo'
      }
    }

    stage('Smoke') {
      steps {
        echo 'Run 10 Testcases'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Move the build'
        echo 'Start the server'
        echo ' Notify Email'
      }
    }

    stage('Integration Testing') {
      parallel {
        stage('Integration Testing') {
          steps {
            echo 'UI Testing'
          }
        }

        stage('API Test') {
          steps {
            echo 'Run Rest Automation'
          }
        }

        stage('Performance Testing') {
          steps {
            echo 'Run Jmeter'
          }
        }

      }
    }

    stage('Certify') {
      steps {
        echo 'QA team certified'
      }
    }

  }
}