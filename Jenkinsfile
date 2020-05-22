pipeline {
  agent any

  stages {
    stage('Build') {
      steps {
        echo 'Building..'
      }
    }
    stage('Test') {
      steps {
        echo 'Testing..'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploying....'
      }
    }
  }
  
  post {
    always {
      echo '"无论如何都会调用"'
    }
    success {
      echo '"只有成功才会调用"'
    }
    failure {
      echo '"只有失败才会调用"'
    }   
  }
}
