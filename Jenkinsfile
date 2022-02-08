pipeline{
  agent any
  options {
    buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '5', daysToKeepStr: '1', numToKeepStr: '5')
    disableConcurrentBuilds()
  }
  stages {
  stage('Hello'){
    steps {
      echo "hello"
    }
  }
  stage('cat hello'){
    steps {
      sh '''
      cat README.md 
      '''
    }
  }  
}
}
