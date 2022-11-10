pipeline {
  agent any
  stages {
    stage('') {
      steps {
        sh '''#!/bin/bash
echo "Printing text with newline"
echo -n "Printing text without newline"
echo -e "\\nRemoving \\t backslash \\t characters\\n"'''
      }
    }

  }
  environment {
    test = '1'
  }
}