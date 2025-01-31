pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        echo 'stage1 completed'
      }
    }

    stage('stage2') {
      steps {
        echo 'stage2 completed'
      }
    }

    stage('stage3') {
      parallel {
        stage('stage3') {
          steps {
            echo 'stage3 parallele'
          }
        }

        stage('stage31') {
          steps {
            echo 'stage31 completed'
          }
        }

        stage('stage32') {
          steps {
            echo 'stage32 completed'
          }
        }

      }
    }

    stage('stage4') {
      steps {
        echo 'stage4 completed'
      }
    }

  }
}