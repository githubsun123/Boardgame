pipeline {
    agent any  < any vm's
    
    tools {
        maven 'maven3.6'  #added as plugin so should define it, same name as in tools
        jdk 'jdk17'
    }    

    stages {
   
        stage('Compile') {
            steps {
                sh 'mvn compile'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('Package') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
