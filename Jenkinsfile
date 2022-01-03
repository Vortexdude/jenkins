pipeline {
    agent any 
    stages {
        stage('Dev') {
            steps {
                echo "You Select ${state}"
            }
        }
        stage('UAT'){
            // when { expression { return env.BRANCH_NAME == 'jenkings' } }
            steps {
                echo "it runs whne the code the pushed to the github "
            }
        }
    }
}