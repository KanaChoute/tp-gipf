node {
  stage('SCM') {
    checkout scm
  }
  stage('test') {
    steps {
      sh 'gradle run test'
    }
  }
  stage('couverture jacoco') {
  }
  stage('sonarqube') {
  }
  stage('jar') {
  }
}
