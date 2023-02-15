node {
  stage('Build') {
    sh 'g++ -o PES2UG20CS321 PES2UG20CS321.cpp'
  }

  stage('Test') {
    sh './PES2UG20CS321'
  }

  stage('Deploy') {
    // Add your deploy step here
  }

  post {
    always {
      if (currentBuild.result == "FAILURE") {
        echo 'Pipeline Failed'
      }
    }
  }
}