pipeline{

    agent any 

    stages{

        stage('Git Checkout'){
           
            steps{

                script{
                 
                 git branch: 'main', credentialsId: 'GitCred', url: 'https://github.com/shankyz/Sampletest.git'

                }
            }
        }

        stage('Maven Build'){

             steps{

              script{
                   
                   sh 'mvn clean install'

                }
             }
        }
}
}
