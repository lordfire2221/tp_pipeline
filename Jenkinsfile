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
            sh 'cd /home/lordfire/tp_pipeline/'

            sh 'pandoc README.md -s -o index1.docx'

          }
        }

      }
    }

  }
}
