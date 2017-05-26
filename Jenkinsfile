pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'i\'m building'
        sleep 3
      }
    }
    stage('testing') {
      steps {
        parallel(
          "testing": {
            echo 'i\'m testing'
            
          },
          "more testing AGAIN": {
            sleep 5
            
          }
        )
      }
    }
    stage('now deploy') {
      steps {
        echo 'deploying'
      }
    }
    stage('production.....') {
      steps {
        echo 'deploying into production'
      }
    }
  }
}
