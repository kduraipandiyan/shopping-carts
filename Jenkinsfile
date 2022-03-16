pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
   tools{
       maven 'maven' 
    }
   

    stages{
        stage('compile'){
            steps{
                echo 'this is the compile job'
                sh 'mvn compile'
               
            }
        }
        stage('test'){
            steps{
                echo 'this is the test job'
                sh 'mvn test'
               
            }
        }
        stage('package'){
            steps{
                echo 'this is the package job'
                sh 'mvn package'
                
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline has completed for shopping cart...### First step done'
        }
        
    }
    
}
