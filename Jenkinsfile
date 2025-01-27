pipeline {
    agent any
    environment { 
    DOCKER_ID = "heuzef"
    DOCKER_IMAGE = "dsapi"
    DOCKER_TAG = "v.${BUILD_ID}.0" 
    }
    stages {
        stage('Building') {
            steps {
                sh 'pip install -r requirements.txt'
            }
        }
        stage('Testing') {
            steps {
                sh 'python -m unittest'
            }
        }
          stage('Deploying') {
              script {
                  
            }
        }
    }
}
