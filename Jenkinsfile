pipeline {
    agent any
    stages {
        stage("Upload to AWS") {
            steps {
                withAWS(region:'us-east-2',credentials:'aws-static') {
                    // do something
                    s3Upload(file:'index.html', bucket:'jenkins-test-aws-static-noah-ross', path:'./index.html')
                }
            }
        }
    }
}