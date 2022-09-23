pipeline{
    agent{
        label{
            label "java-slave"
        }
    }
    tools{
        maven "M2_HOME"
    }
    stages{
        

        stage('Build'){
            steps{
                sh 'mvn clean install package'
            }
        }
    }
}
