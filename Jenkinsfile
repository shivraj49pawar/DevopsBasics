pipeline {
  agent any
  stages {
    stage('Hello') {
      steps {
        echo 'Hello Abhishek'
      }
    }

    stage('Build_job') {
      steps {
        build(job: 'Test_10112022', quietPeriod: 1, propagate: true, wait: true)
      }
    }

  }
}