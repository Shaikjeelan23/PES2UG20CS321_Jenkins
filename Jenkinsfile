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
       sh './PES2UG20CS321'
    }
  }

  stage('Deploy') {
//steps here
  }
  }

  post {
    failure {
        echo 'Pipeline Failed'
    }
  }
}
