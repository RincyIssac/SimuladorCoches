pipeline { 
    agent any 
    stages { 
        stage('Checkout') { 
            steps { 
                git branch : 'master', url: 'https://github.com/RincyIssac/SimuladorCoches'
                bat 'dir'
                
            } 
            
        }        
        stage('Compile') { 
            steps { 
                 
                dir ('standalone'){
                    bat 'dir'
                    bat 'mvn clean compile'
                   
                }
                
            } 
            
        } 
        stage('Test') { 
            steps { 
                echo 'Testing...' 
                
            } 
            
        } 
        stage('Package') { 
            steps { 
                echo 'Packaging...'                
                
            } 
            
        } 
        stage('Acceptance test') { 
            steps { 
                echo 'Acceptance...' 
                
            } 
            
        } 
        stage('Deploy') { 
            steps { 
                echo 'Deploying....' 
                
            } 
            
        } 
        
    } 
    
}
