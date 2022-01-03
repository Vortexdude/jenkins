pipeline {
    agent any 
    stages {
        stage('Dev') {
            steps {
                echo "You Select ${state}"
            }
        }
        stage('UAT'){
            when { expression { return env.BRANCH_NAME == 'jenkings' } }
            steps {
                echo "it runs when the branch name is jenkings  "
            }
        }
        stage('deploy'){
            when { expression { return Deploy == 'true' } }
            steps {
                echo "You Deploy with the ${env.BRANCH_NAME}"
            }

        }
    }
}