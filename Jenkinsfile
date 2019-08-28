pipeline {
  agent any
  stages {
    stage('SCM') {
      steps {
        git(url: 'https://github.com/gowdilyan/NewApp.git', branch: 'master')
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