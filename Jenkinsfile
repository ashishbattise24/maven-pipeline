pipeline{
 agent any
 
 parameters{
            choice(name: 'VERSION', choices: ['1.2.3', '1.2.4' ,'1.2.5'], description: 'Version choises' )
            booleanParam(name: 'execValue, defaultValue: true, description: 'Boolean parameter')
 }
 stages{
    stage('Build'){
    
                steps{
                       echo "${VERSION}"
                     }
 
 
                 }
    stage('Prod'){
                 steps{
                     when {
                         expression{
                                 params.execValue
                                   }
                          }
                     }
 
                 }

}
}
