pipeline {
       agent any
 stages {
     stage("Compile stage"){
       steps {
       
               withMaven(mmaven:"maven_3_5_2"){
                 sh "mvn clean compile"
                 }
               }  
          }
          stage("Testing stage"){
            steps {
                   withMaven(mmaven:"maven_3_5_2")  {
                             sh "mvn test"
                             }
                             }
         }
         
         stage("Deploy stage"){
         steps {
       
               withMaven(mmaven:"maven_3_5_2"){
                 sh "mvn clean compile"
                 }
               }  
          }          
   }
}     
