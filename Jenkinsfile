pipeline {
    agent any
    parameters {
  choice choices: ['1.10', '1.20', '1.30'], description: 'Selecting the version', name: 'VERSION'
  booleanParam defaultValue: true, description: 'checking and execute', name: 'check'
        


    stages {
        stage('build') {
            when{
                expression{
                    params.execute
                }
            }
   
            steps {
                echo 'building the application'
            }
        }
    
   
        stage('test') {
   
            steps {
                echo 'testing the application'
                echo " the version for testing is ${params.VERSION}"
                
            }
        }
    

        stage('deploy') {
   
            steps {
                echo 'deploying the application'
            }
        }
    }
}
