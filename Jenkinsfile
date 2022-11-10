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
        build(job: 'DevopsBasics', quietPeriod: 1, propagate: true, wait: true)
      }
    }

  }
}