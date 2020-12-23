pipeline {
   agent any
   //Funcion para monitorear cambios dentro del repositorio
   /*triggers {
        pollSCM('* * * * *')
   }*/
   
   stages { 
          /*stage('clean') { 
                     steps { 
                            bat 'gradlew clean'
                            bat 'dir'
                     }
         }
         stage('build') { 
                     steps { 
                            bat 'gradlew build'
                     }
         }*/
         stage('Release') { 
                     steps { 
                            bat 'gradlew AssembleRelease'
                     }
                     //Funcion para enviar por correo
                     /*post {
                        success {
                            echo 'AWESOME SUCCESS!'
                            emailext body: 'New Update Available', recipientProviders: [[$class: 'DevelopersRecipientProvider'], [$class: 'RequesterRecipientProvider']], subject: 'New Update!'
                        }
                     
         }*/
    }
    //Funcion dentro de gradle para realizar escaneo sin necesidad de jenkins
         /*stage('Sonar') { 
                     steps { 
                            bat 'gradle sonarqube'
                     }
         }*/
   }
}
