pipeline {
    agent any
    stages {
        stage('Upload to AWS.') {
            steps {
                withAWS(region:'us-west-2',credentials:'AKIAWGGR4EKL7JDD2PHX') {
                    s3Upload(file:'index.html', bucket:'jenkins-project', path:'index.html')
                }
            }
        }
    }
}
