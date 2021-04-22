pipeline{
 agent any
 environment {
         PKG_VERSION = '1.1.3'
 }
 server_credential = credentials('server-credential')
 stages{
    stage('Build'){
    
                    steps{
                           echo "${PKG_VERSION}"
                           echo "${server_credential}"
           }

             post{
                   success{

                     echo "Now Archiving Artifact...."
                   }
              
             }     

 
    }
 }

}
