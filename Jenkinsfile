pipeline {
    agent {
        docker {
            image 'node:lts-bullseye-slim' 
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh "cd /var/lib/jenkins/workspace/react-app && npm install ."
            }
        }
    }
}
