pipeline{
    agent any
    stages {
        stage ('Build'){
            steps{
                sh 'docker build -t hello-devops .'
            }
        }
        stage ('Run Container'){
            steps{
                sh 'docker run -d -p 5000:5000 hello-devops'
            }
        }
    }
}