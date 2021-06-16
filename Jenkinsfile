pipeline {
  agent {
    node {
      label 'master'
    }

  }
  environment {
    DEMO = '1.3'
  }
  stages {
    stage('stage-1') {
      steps {
        echo "This is build $BUILD_NUMBER of demo $DEMO"
        sh '''
            echo "Using a multiline shell step"
            chmod +x test.sh
            ./test.sh
           '''
      }
    }

  }
  
}
