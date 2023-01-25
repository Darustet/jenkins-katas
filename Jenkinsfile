pipeline {
  agent any
  stages {
    stage('Parallel execution') {
      parallel {
        stage('Say Hello') {
          steps {
            sh 'echo "Hello World!"'
          }
        }

        stage('build app') {
          agent any
          steps {
            sh 'sh \'echo Building\''
          }
        }

      }
    }

  }
  environment {
    demo = '1'
  }
}