pipeline {
    agent any
    stages {
    stage('maven install') {
      steps {
    withMaven(globalMavenSettingsConfig: '--- Use system default settings or file path ---', jdk: 'OpenJDK', maven: 'Maven3', mavenSettingsConfig: '--- Use system default settings or file path ---') {
        sh 'mvn clean install'
    }
      }
    }

  }
}
