node {
  stage('SCM') {
    checkout scm
  }
  stage('test') {
    steps {
      gradle 'npm run test'
    }
  }
  stage('couverture jacoco') {
  }
  stage('sonarqube') {
  }
  stage('jar') {
  }
}
