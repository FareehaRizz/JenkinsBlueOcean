pipeline {
  agent any
  stages {
    stage('Building Stage') {
      parallel {
        stage('Building Stage') {
          steps {
            echo 'Here the code will be built'
          }
        }

        stage('Parallel Building Stage') {
          steps {
            echo 'Here, parallel building of some other piece of code will take place.'
          }
        }

      }
    }

    stage('Testing Stage') {
      parallel {
        stage('Testing Stage') {
          steps {
            echo 'Here the built code will be tested.'
          }
        }

        stage('Parallel Testing Stage') {
          steps {
            echo 'Parallel testing of another piece of code'
          }
        }

      }
    }

    stage('Deployment Stage') {
      steps {
        echo 'Here the application will be Deployed'
      }
    }

  }
}