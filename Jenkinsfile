pipeline{
    agent any

    tools{
        maven 'm3'
        jdk "jdk9"
    }

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