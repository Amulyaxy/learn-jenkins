pipeline {
        agent{
            node{
                label 'AGENT-1'
            }
        }
        stages('Build') {
            steps {
                echo 'Building..'
            }
        }
        stages('Test') {
            steps {
                echo 'Testing'
            }
        }
        stages('Deploy') {
            steps {
                echo 'Deploying...'
            }
        }
}
    

