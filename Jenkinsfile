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
                sh "HOME=${WORKSPACE} && cd ${WORKSPACE}/src/common && some command"
            }
        }
    }
}
