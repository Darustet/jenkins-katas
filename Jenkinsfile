pipeline {
  agent any
  stages {
    stage('Parallel execution') {
      parallel {
        stage('Say Hello') {
          steps {
            sh 'echo "Hello World!"'
            archiveArtifacts 'text.txt'
          }
        }

        stage('build app') {
          agent any
          steps {
            sh 'touch text.txt'
          }
        }

      }
    }

  }
  environment {
    demo = '1'
  }
}