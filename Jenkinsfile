pipeline {
  agent any
  stages {
    stage('get SCM') {
      steps {
        git(url: 'https://github.com/gopaldevops7/spring3-mvc-maven-xml-hello-world.git', branch: 'master', changelog: true, poll: true, credentialsId: 'gopaldevops7')
      }
    }

    stage('build MAVEN') {
      steps {
        sh 'maven packege'
      }
    }

  }
}