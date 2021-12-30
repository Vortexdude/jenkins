pipeline {
    agent any 
    stages {
        stage('Dev') {
            steps {
                echo "You Select ${state}"
            }
        }
        stage('test'){
            steps {
                if ${Runner}{
                    echo "You Run with Runner"
                }else
                echo 'You simply run'
            }
        }
            }
}