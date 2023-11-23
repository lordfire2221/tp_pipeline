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
            sh '''cd tp_pipeline
pandoc READEME.md -s -o .index.docx
'''
          }
        }

      }
    }

  }
}