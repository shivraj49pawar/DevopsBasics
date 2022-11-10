pipeline {
  agent any
  stages {
    stage('Hello') {
      parallel {
        stage('Hello') {
          steps {
            echo 'Hello Abhishek'
          }
        }

        stage('') {
          steps {
            timestamps()
          }
        }

      }
    }

    stage('Build_job') {
      steps {
        build(job: 'DevopsBasics', quietPeriod: 1, propagate: true, wait: true)
      }
    }

  }
}