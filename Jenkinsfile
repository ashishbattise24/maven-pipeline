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
                       withCredential([
                        usernamePassword( credential: 'server-credential', usernameVariable: USER, passwordVariable: PWD)
                        sh "id ${USER}"    
                      ]){

}
           }

             post{
                   success{

                     echo "Now Archiving Artifact...."
                   }
              
             }     

 
    }
 }

}
