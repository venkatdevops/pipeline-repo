pipeline {
    agent any

    stages {
        stage ('Clean ') {

            steps {
                withMaven(maven : 'mvn') {
                    sh 'mvn clean'
                }
            }
        }

        stage ('complie') {

            steps {
                withMaven(maven : 'mvn') {
                    sh 'mvn compile'
                }
            }
        }


        stage ('test-compile') {
            steps {
                withMaven(maven : 'mvn') {
                    sh 'mvn test-compile'
                }
            }
               }
    
    
    stage ('package') {
            steps {
                withMaven(maven : 'mvn') {
                    sh 'mvn package'
                }
            }
}
    stage ('deploy') {
            steps {
                withMaven(maven : 'mvn') {
                    sh 'mvn deploy'
                }
            }
}
    
    
    
    
    }
    
    
}
