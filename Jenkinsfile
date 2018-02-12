pipeline{
    agent {label 'large'}
    stages{
        stage('Build stage'){
            steps {
                echo 'Building the application'
            }
        }
        stage ('Test Stage'){
            steps {
                echo 'Testing the application'
                sleep 10
                
            }
        }
        stage('Deploy stage'){
            steps {
                echo 'Deploying the applicaton'
            }
        }
    }
    post {
        always {
            echo 'post action alleways happens'
        }
        failure {
            echo "failed"
        }
        success {
            echo 'we have succeeded'
            
        }
        aborted {
            echo 'Build ' .  ${env.BUILD_NUMBER} . ' has been aborted'
        }
    
    }
}
