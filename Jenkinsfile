pipeline{
  agent any
  stages{
  stage('Build') {
    steps{
      sh 'g++ -o PES2UG20CS321 PES2UG20CS321.cpp'
    }
  }

  stage('Test') {
    steps{
       sh './PES2U'
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
