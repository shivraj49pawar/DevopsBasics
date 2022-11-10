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
            sh '''#!/bin/bash
valid=true
count=1
while [ $valid ]
do
echo $count
if [ $count -eq 5 ];
then
break
fi
((count++))
done'''
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