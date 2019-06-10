pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building..'
        git branch: 'master',
          credentialsId: 'afafa50b-6687-45e3-a6a5-e36dfe01c998',
          url: 'https://github.com/wayneseymour/hello-jenkinsfile.git'
      }
    }
    stage('Test') {
      steps {
        echo '\n\t### Some Testing..'
        sh './some-file.sh'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploying....'
      }
    }
  }
}
