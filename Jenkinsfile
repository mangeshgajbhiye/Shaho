pipeline {
      
     agent any
     
     stages{
        
        stage('Checkout') {
            
             steps {
                   checkout scm
              }
         }
        stage('Build') {
             
             steps {
               sh '/home/mangesh/Software/apache-maven-3.6.1/bin/mvn install'
              }
         }
        stage('Deployment') {
          
             steps {
               sh 'cp target/shaho.war /home/mangesh/Software/apache-tomcat-8.5.43/webapps' 
              }
         }
      }
}
