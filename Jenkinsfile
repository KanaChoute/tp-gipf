node {
  stage('SCM') {
    checkout scm
  }
  stage('update') {
    steps {
      sh './gradlew -D https.proxy.Host=proxy1-rech'
      sh './gradlew -D https.proxy.Port=3128'
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
