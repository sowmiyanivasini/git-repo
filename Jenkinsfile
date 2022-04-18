pipeline {
  agent any
  stages {
    stage('stage1') {
      parallel {
        stage('stage1') {
          steps {
            sh 'echo "From stage1"'
          }
        }

        stage('parallel_stage1.1') {
          steps {
            sh 'echo "Hello parallel stage2.1"'
          }
        }

      }
    }

    stage('stage2') {
      parallel {
        stage('stage2') {
          steps {
            sh 'echo "From stage2"'
            sleep 5
            sh 'echo "script after sleep"'
          }
        }

        stage('parallel_stage2.2') {
          steps {
            sh 'echo "Hello from parallel stage2.2"'
            sleep 5
          }
        }

      }
    }

  }
}