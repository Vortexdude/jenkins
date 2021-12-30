pipeline {
    agent any 
    stages {
        stage('Stage 1') {
            steps {
                echo 'Hello world!' 
            }
        }
        stage('Stage 2'){
            steps {
                sh cd src && bash new.sh
            }
        }
    }
}
