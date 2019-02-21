pipeline {
    agent any
    
    tools   {
        maven "Maven"
        jdk "Java 8"
    }

    stages {
        stage ('Compile Stage') {

            steps {
                
                    sh "mvn clean"
                
            }
        }

        stage ('Testing Stage') {

            steps {
                
                    sh "mvn test"
                
            }
        }


       
    }
}
