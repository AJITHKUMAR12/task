pipeline {
    agent any

    stages {
        stage('Build') {
            when{
                expression{
                     BRANCH_NAME == 'main'
                    echo 'tset pass'
                }
                
            }
            steps {
                echo 'Building the application'
            }
        }
 stage('test') {
     when{
                expression{
                     BRANCH_NAME == 'master'
                    echo 'test pass'
                }
                
            }
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
