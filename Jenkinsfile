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
        stage('deploy'){
            when { expression { return ${Runner} == 'true' } }
            steps {
                echo "You run with the runner with branch ${env.BRANCH_NAME}"
            }

        }
    }
}