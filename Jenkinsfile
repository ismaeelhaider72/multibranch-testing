pipeline{
  agent any
  options {
    buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '5', daysToKeepStr: '1', numToKeepStr: '5')
    disableConcurrentBuilds()
  }
  stages('Hello'){
    steps {
      echo "hello"
    }
  }
}
