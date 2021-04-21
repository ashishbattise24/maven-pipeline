pipeline{
 agent any
 Environment {
         PKG_VERSION = '1.1.3'
 }
 stages{
    stage('Build'){
    
                    steps{
                           echo "${PKG_VERSION}"
           }

             post{
                   success{

                     echo "Now Archiving Artifact...."
                   }
              
             }     

 
    }
 }

}
