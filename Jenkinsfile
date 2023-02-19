pipeline {
    agent any

stages{
  stage('Build') {
    steps{
      sh 'g++ -o woring working.cpp'
    }
  }

  stage('Test') {
    steps{
       sh './working'
    }
  }

  stage('Deploy') {
    steps{
      echo 'DEPLOYMENT SUCCESSFUL'
    }
  }
}
post {
    failure {
        echo 'Pipeline Failed'
    }
  }
}

