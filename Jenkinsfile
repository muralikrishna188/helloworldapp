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
        stage('Archive and Test results'){
            steps {
               junit '**/surefire-reports/*.xml'
               archiveArtifacts artifacts: '**/*.war', followSymlinks: false
            }
        }
    }
}
