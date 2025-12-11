pipeline {          
    agent any         
    
    stages {        
        
        stage('Git Checkout') {  
            steps {
                git branch: 'build1', credentialsId: 'ssh_local_v_oct17_ID', url: 'https://github.com/VeronicaJeya/webhook-repo.git' 
                
            }
        }
        
        stage('Build') {
            steps {
                sh '''
                             
                    python3 list_akanksha.py                                         
                '''
                
            }
        }
    }
    
   
            
}
