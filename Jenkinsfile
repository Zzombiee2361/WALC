pipeline {
  agent {
    docker {
      image 'node:lts'
    }

  }
  stages {
    stage('Install Dependencies') {
      agent {
        node {
          label 'any'
        }

      }
      steps {
        sh 'npm install'
      }
    }

    stage('Dist Linux') {
      agent {
        node {
          label 'any'
        }

      }
      steps {
        sh 'npm run dist'
      }
    }

  }
}