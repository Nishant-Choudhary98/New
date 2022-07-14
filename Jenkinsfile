pipeline {
    agent {
         docker {
               //This image parameter (of the agent section’s docker parameter) downloads the python:3.8
               //Docker image and runs this image as a separate container. The Python container becomes
               //the agent that Jenkins uses to run the Build stage of the Pipeline project.
               image 'python:3.8.3'
                }
            }
    stages {
        stage('build') {
            steps {
                bat 'python hello.py'           
            }
        }
     }
   }
