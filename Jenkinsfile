pipeline{
    agent {docker 'maven:3.5-alpine'}
    stages{
        
        
        stage('checkout'){
            
            steps{
                git 'https://github.com/samsubbiah/spring-petclinic.git'
                sh 'mvn --version'
            }
        }
        
        stage('build'){
          
            steps{
               sh 'mvn clean package'
               
            }
        }
    }
    
    
    
}


