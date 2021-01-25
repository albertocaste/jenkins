pipeline {
  agent any
  stages {
    stage("build") {
      steps {
        echo "ouuuhh mama"
      }
    }
    stage("test") {
      when {
        expression {
          BRANCH_NAME == "dev" || BRANCH_NAME == "master"
        }
      }
      steps {
       echo "ouuuhh papa"
      }
    }
    stage("deploy") {
      steps {
        echo "just kill the man"
      }
    }
  }
  post {
    always {
      echo "esto siempre va a ocurrir"
    }
    failure {
      echo "algo fallo pendejo"
    }
  }
}
