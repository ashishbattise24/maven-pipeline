pipleline{
 agent any
 stages{
    stage('Build Application'){
    
                    steps{
                         sh 'mvn clean package'
           }
             post{
                   success{

                     echo "Now Archiving Artifact...."
                     archiveArtifacts artifacts '**/*.war'
                   }
              
             }     

       }
 
    }
 }

}
