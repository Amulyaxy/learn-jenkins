pipeline {
        agent{
            node{
                label 'AGENT-1'
            }
        }
        environment { 
            GREETING = 'Hello Jenkins'
        }
        options {
            timeout(time: 1, unit: 'SECONDS')
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
                sh """
                    echo "Here I wrote shell script"
                    echo "$GREETING"
                """
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
    

