pipeline{
    agent{
        label "jenkins"
    }
    stages{
        stage("Build"){
            steps{
                echo "========executing Build========"
            }
        }
        stage("Test"){
            steps{
                echo "====++++executing Test++++===="
            }
        }
        stage("Deploy"){
            steps{
                echo "====++++executing Deploy++++===="
            }
        }
    }
    post{
        always{
            echo "========always========"
        }
        success{
            echo "========pipeline executed successfully ========"
        }
        failure{
            echo "========pipeline execution failed========"
        }
    }
}