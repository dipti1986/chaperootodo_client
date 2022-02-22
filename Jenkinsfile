pipeline{
        agent any
        stages{
            stage('Install Docker'){
                steps{ "sudo chmod 755 ./install-docker.sh"
                    sh "./install-docker.sh"
                }
            }
            stage('Run App'){
                steps{
                    sh "sudo docker-compose up -d --build"
                }
            }
        }    
}
