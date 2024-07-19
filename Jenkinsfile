pipeline {
    agent any
    parameters{
        choice(name:'version',choices['1.10','1.20','1.30'],description: '')
        booleanParam (name :'execute',defaultvale : True,description:'')
    }

    stages {
        stage('Build') {
          
            steps {
                echo 'Building the application'
                echo "deploying the version $(params.version)" 
            }
        }
 stage('test') {
     when{
         expression{
             params.excute
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
