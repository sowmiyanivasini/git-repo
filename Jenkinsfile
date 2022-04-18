pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        sh 'echo "From stage1"'
      }
    }

    stage('stage2') {
      steps {
        sh 'echo "From stage2"'
        sleep 5
        sh 'echo "script after sleep"'
      }
    }

  }
}