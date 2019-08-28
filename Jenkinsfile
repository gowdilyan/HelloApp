pipeline {
  agent any
  stages {
    stage('SCM') {
      steps {
        sh 'git clone https://github.com/gowdilyan/NewApp.git'
      }
    }
    stage('list') {
      steps {
        sh 'ls -lrth'
      }
    }
    stage('build') {
      steps {
        sh 'mvn clean install'
      }
    }
  }
}