pipeline {
    agent any
    stages{
        stage('system statistics and Jenkins status check'){
            parallel{
                stage('Max'){
                    steps{
                        sh "lscpu"
                         sh "sudo systemctl status jenkins"
                    }
                }
                stage('Christianah'){
                    steps{
                        sh "lscpu"
                        sh "sudo systemctl status jenkins"
                    }
                }
            }
        }
        stage('End of parallel build'){
            steps{
                echo "End of pipeline"
            }
        }
    }
}
