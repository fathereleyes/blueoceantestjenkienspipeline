pipeline {
  agent any
  stages {
    stage('1') {
      steps {
        echo '111'
      }
    }

    stage('2') {
      steps {
        echo '2'
      }
    }

    stage('3') {
      steps {
        echo '3'
      }
    }

    stage('4') {
      steps {
        echo '4'
      }
    }

    stage('5') {
      steps {
        echo '5'
      }
    }

    stage('6') {
      parallel {
        stage('6') {
          steps {
            input(message: 'r u sure u want', id: 'xxc', ok: 'xbxc', submitter: 'xcbx', submitterParameter: 'xbxcnz')
            echo '6'
            retry(count: 3)
            sh 'no'
          }
        }

        stage('error') {
          steps {
            input(message: '5555555', id: '555555', ok: '55555555', submitter: '1', submitterParameter: '2')
          }
        }

      }
    }

  }
}