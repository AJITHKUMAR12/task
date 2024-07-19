pipeline {
    agent any

    stages {
        stage('Build') {
            when{
                expression{
                    // BRANCH_NAME == 'master'
                    environment name: 'BRANCH_NAME', value: 'master'
                    echo 'tset pass'
                }
                 steps {
                echo 'checking the application'
            }
                
            }
            steps {
                echo 'Building the application'
            }
        }
 stage('test') {
    
            steps {
                echo 'testing the application'
            }
        }
 stage('Deploy') {
            steps {
                echo 'Deploy the application'
            }
        }

    }
}
