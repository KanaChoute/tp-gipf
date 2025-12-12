node {
  stage('SCM') {
    checkout scm
  }
  stage('update') {
    steps {
      sh 'npm ci'
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
