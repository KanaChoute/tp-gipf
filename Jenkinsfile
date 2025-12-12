node {
  stage('SCM') {
    checkout scm
  }
  stage('update') {
    steps {
      sh 'npm update'
    }
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
