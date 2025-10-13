pipeline {
  agent any
  stages {
    stage('SCM') {
      steps {
        echo '>>>>>  stage \'SCM\' is commplete.............. from blueocean'
      }
    }

    stage('Build') {
      steps {
        echo '>>>>>  stage \'Build\' is commplete..........'
      }
    }

    stage('Test1') {
      parallel {
        stage('Test1') {
          steps {
            echo '>>>>>  stage \'Test1\' is commplete...........'
          }
        }

        stage('Test2') {
          steps {
            echo '>>>>>  stage \'Test2\' is commplete...........'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        input(message: 'you want to deploy ?', cancel: 'no', ok: 'yes')
        echo '>>>>>  stage \'Deploy\' is commplete........." '
      }
    }

  }
}