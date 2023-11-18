pipeline {
    agent any

    stages {
        stage('Git') {
            steps {
                git 'https://github.com/jaiswaladi2468/BoardgameListingWebApp.git'
            }
        
        }
   
        stage('Compile') {
            steps {
                sh 'mvn compile'
            }
        }
        
        
        
         
        stage('Test') {
            steps {
               sh 'mvn clean test'
            }
        
        }
        
         
        stage('Package') {
            steps {
                 sh 'mvn clean package'
            }
        
        }
            
        stage('Docker') {
            steps {
                echo "Docker Started"
            }
        }
        
    }
}
              
         
