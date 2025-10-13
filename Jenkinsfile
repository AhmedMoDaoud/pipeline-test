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

    stage('Test') {
      steps {
        echo '>>>>>  stage \'Test\' is commplete...........'
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