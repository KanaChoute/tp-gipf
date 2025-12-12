node {
  stage('SCM') {
    checkout scm
  }
  stage('gradle') {
    sh './gradlew 
    -Dhttps.proxyHost=proxy1-rech \
    -Dhttps.proxyPort=3128'
  }
  stage('sonarqube') {
      sh './gradlew sonar \
  -Dsonar.projectKey=tp-gipf \
  -Dsonar.projectName='tp-gipf' \
  -Dsonar.host.url=http://127.0.0.1:9000 \
  -Dsonar.token=sqp_593c03e1f2b8e26c034f5afb1c0b083e7408afc9 \
  }
  stage('jar') {
    sh 'make' 
    archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true
  }
}
