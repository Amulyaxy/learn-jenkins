pipeline {
        agent{
            node{
                label 'AGENT-1'
            }
        }
    stages{
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
   
        stage('Test') {
            steps {
                echo 'Testing'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
            }
        }
    }
    post { 
        always {
            echo 'I will alwasy say hello!'
        }
        failure {
            echo 'this is run when pipelines failed, used generallt to send some alerts'
        }
        success {
            echo 'I will say hello pipeline is success'
        }
    }
}
    

