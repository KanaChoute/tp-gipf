node {
  stage('SCM') {
    checkout scm
  }
  stage('test') {
    steps {
      sh 'npm run test'
    }
  }
  stage('couverture jacoco') {
  }
  stage('sonarqube') {
  }
  stage('jar') {
  }
}
