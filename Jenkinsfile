pipeline{
    agent any
        
    
    tools{
        maven "M2_HOME"
    }
    stages{
        

        stage('Build'){
            steps{
                sh 'mvn clean install package'
            }
        }

        stage("Deploy application") { 
            steps { 
               sh 'echo "deploying application..."'
         }

     }       
    }
}
