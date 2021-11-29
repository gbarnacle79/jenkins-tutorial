pipeline{
        agent any
        stages{
            stage('Run App'){
                steps{
                    sh "sudo docker-compose up -d --build"
                }
            }
        
            stage('Make Directory'){
                steps{
                    sh "mkdir ~/jenkins-tutorial-test"
                }
            }
            stage('Make Files'){
                steps{
                    sh "touch ~/jenkins-tutorial-test/file1 ~/jenkins-tutorial-test/file2"
                }
            }
        }
}
