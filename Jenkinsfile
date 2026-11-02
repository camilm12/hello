pipeline {
  agent any

  stages {
    steps {
      git branch: 'main',
        url: 'git@github.com:camillm12/hello.git',
        credentialsId: 'github-ssh'
    }
  }

  stage('Build') {
    steps {
      bat 'mvn clean package'
    }
  }
}
