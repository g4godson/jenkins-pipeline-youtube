pipeline {
    agent any
    
    tools   {
        maven 'maven'
        jdk 'Java 8'
    }

    stages {
        stage ('Compile Stage') {

            steps {
                
                    bat "mvn clean"
                
            }
        }

        stage ('Testing Stage') {

            steps {
                
                    bat "mvn test"
                
            }
            
            
        }


       
    }
}
