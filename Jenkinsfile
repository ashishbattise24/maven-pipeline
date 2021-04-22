pipeline{
 agent any
 environment {
         PKG_VERSION = '1.1.3'
         SERVER_CREDENTIAL = credentials('server-credential')
 }
 stages{
    stage('Build'){
    
                    steps{
                           echo "${PKG_VERSION}"
                           echo "${SERVER_CREDENTIAL}"
           }

             post{
                   success{

                     echo "Now Archiving Artifact...."
                   }
              
             }     

 
    }
 }

}
