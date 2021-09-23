pipeline {
  agent any
  stages {
    stage('build-the-app') {
      steps {
        echo 'this is the build job'
        sh 'npm install'
      }
    }

    stage('test-the-app') {
      steps {
        echo 'this is the test job'
        sh 'npm test'
      }
    }

    stage('package-the-app') {
      steps {
        echo 'this is the package job'
        sh 'npm run'
      }
    }

<<<<<<< HEAD
    stages{
        stage('build-the-app'){
            steps{
                echo 'this is the build job'
                sh 'npm install'
            }
        }
        stage('test-the-app'){
            steps{
                echo 'this is the test job'
                sh 'npm test'
            }
        }
        stage('package-the-app'){
            steps{
                echo 'this is the package job'
                sh 'npm run package'
            }
        }
=======
    stage('archive-the-app') {
      steps {
        archiveArtifacts '**/distribution/*.zip'
      }
>>>>>>> 4319429adbb1d8c5ff29c507baa3608eda8ce1f7
    }

  }
  tools {
    nodejs 'nodejs'
  }
  post {
    always {
      echo 'this pipeline has completed...'
    }

  }
}