pipeline {
  agent {
    docker {
      args '-p 3000:3000'
      image 'node:6-alpine'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh '''echo -n "Npm Version:"
npm --version
echo -en "\\nNode Version:"
node --version
npm install'''
      }
    }
  }
}