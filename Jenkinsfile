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
               echo "This is test stage"
            }
        }
        stage('UAT'){
            when { expression { return env.BRANCH_NAME == 'jenkings' } }
            steps {
                echo "it runs when the branch name is jenkings"
            }
        }
        stage('deploy'){
            when { expression { return Deploy == 'true' } }
            steps {
                echo "You run with the runner with branch env.BRANCH_NAME"
            }

        }
    }
}