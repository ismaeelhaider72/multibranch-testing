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
  stage('for fix branch'){
    when {
      branch "fix-*"
    }
    steps {
      sh '''
      cat README.md
      cat README.md
      '''
    }
  }
  stage('for PR branches'){
    when {
      branch "PR-*"
    }
    steps {
      sh 'aws dlafsfs'
      echo "this is only for PR branch"
    }
  }   

}
}
