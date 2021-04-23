pipeline{
 agent any
 
 paramerters{
            choice(name: "VERSION", choices: [1.2.3,1.2.4,1.2.5], description: "Version choises" )
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
