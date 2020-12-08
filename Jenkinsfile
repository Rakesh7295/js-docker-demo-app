pipeline{
    agent{
        label "jenkins"
    }
    parameters{
        string(name: 'USER_NAME', defaultValue: 'jenkins', description: 'Enter user name')
        booleanParam(name: 'DEMO', defaultValue: true, description: 'built type')
    }
    stages{
        stage("Build"){
            steps{
                echo "========executing Build========"
                echo "executer name is ${params.USER_NAME}"
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
