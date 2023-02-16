pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                sh 'g++ test.cpp'
                sh '/vaar/jenkins_home/workspace/pes1ug20cs457-1/main/hello_exec'
            }
        }
        stage('Test'){
            steps{
                sh './a.out'
                echo 'Testing'
            }
        }
        stage('Deploy'){
            steps{
                echo 'Deployed successfully'
            }
        }
    }
    post{
        failure{
            echo 'Build failed'
        }
    }
}
