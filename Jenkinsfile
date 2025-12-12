node {
  stage('SCM') {
    checkout scm
  }
  stage('sonarqube') {
      sh './gradlew sonar \
  -Dhttps.proxyHost=proxy1-rech \
  -Dhttps.proxyPort=3128 \
  -Dsonar.projectKey=tp-gipf \
  -Dsonar.projectName='tp-gipf' \
  -Dsonar.host.url=http://127.0.0.1:9000 \
  -Dsonar.token=sqp_7600c6b39f787650b99c00b7e6d94aa465e15fec'
  }
  stage('jar') {
  }
}
