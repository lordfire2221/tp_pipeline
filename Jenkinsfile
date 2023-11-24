pipeline {
  agent any
  stages {
    stage('first') {
      parallel {
        stage('first') {
          steps {
            echo '"hello world"'
          }
        }

        stage('build') {
          steps {
            sh 'pandoc README.md -s -o index1.docx'

          }
        }

      }
    }

  }
}
