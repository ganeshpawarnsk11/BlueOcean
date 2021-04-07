pipeline {
  agent any
  stages {
    stage('Git Check Out') {
      steps {
        git(url: 'https://github.com/ganeshpawarnsk11/BlueOcean.git', branch: 'master')
        echo 'Successfully Checkout from Git'
      }
    }

    stage('Compile') {
      steps {
        bat 'Compile.bat'
        echo 'Compiled Successfully'
      }
    }

    stage('Package') {
      steps {
        bat 'Package.bat'
        echo 'Packaged Successfully'
      }
    }

    stage('Deploy') {
      steps {
        bat 'Deploy.bat'
        echo 'deployed Successfully'
        echo 'Super easy to use the blue ocean UI for pipelline creation'
      }
    }

  }
}