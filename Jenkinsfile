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
          steps {
            sh 'sh \'echo text.txt\''
          }
        }

      }
    }

  }
  environment {
    demo = '1'
  }
}