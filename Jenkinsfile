pipeline{
 agent any
 
 parameters{
            choice(name: 'VERSION', choices: ['1.2.3', '1.2.4' ,'1.2.5'], description: 'Version choises' )
 }
 stages{
    stage('Build'){
    
                steps{
                       echo "${PKG_VERSION}"
                     }
 
 
                 }

}
}
