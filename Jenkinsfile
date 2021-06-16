pipeline{
    agent any
    stages{
        stage('Checkout SCM'){
            agent{
                docker {
                    image 'node'
                }
            }
            steps{
            sh 'npm install'
            sh 'npm build'
            }   
        }
    }
}