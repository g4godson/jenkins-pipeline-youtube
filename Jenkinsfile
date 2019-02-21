pipeline {
    agent any
    
    tools   {
        jdk 'Java 8'
    }

    stages {
        stage ('Compile Stage') {

            steps {
                withMaven(maven : 'maven') {
                    bat 'mvn clean compile'
                }
            }
        }

        stage ('Testing Stage') {

            steps {
                withMaven(maven : 'maven') {
                    bat 'mvn test'
                }
            }
        }


        stage ('Deployment Stage') {
            steps {
                withMaven(maven : 'maven') {
                    bat 'mvn deploy'
                }
            }
        }
    }
}
