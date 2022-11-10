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

        stage('error') {
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

    stage('Post Build steps') {
      steps {
        writeFile(file: 'test_1011.txt', text: 'Hello Woodpecker!!!')
      }
    }

  }
}