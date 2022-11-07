pipeline{
    
    agent any 
    
    stages {
        
        stage('Git Checkout'){
            
            steps{
                    
                    git branch: 'main', url: 'git@github.com:parthu2/demo-counter-app.git'
            }
        }
        stage('Maven build'){
            
            steps{
                    
                    sh 'mvn clean package'
            }
        }
         stage('UNIT testing'){
            
            steps{
                
                script{
                    
                    sh 'mvn test'
                }
              }  
            }
        }
        
}
