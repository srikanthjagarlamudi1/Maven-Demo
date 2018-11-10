pipeline {
    agent any
    stages {
        stage('git') {
        steps {
         git 'https://github.com/pandian3k/Maven-Demo.git'       
        }
        }
        stage('installation') {
            steps {
                bat 'mvn install'
            }
        }
    
        stage('Deployment') {
            steps {
                 sh 'cp -rp "C:\\Program Files (x86)\\Jenkins\\workspace\\pipe_pushpa_01\\multi-module\\webapp\\target\\webapp.war" "C:\\Program Files\\Apache Software Foundation\\Tomcat 8.5\\webapps"'
            }
        }
    }
    
}

