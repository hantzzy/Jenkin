pipeline {
    agent any
    stages {
       stage('Upload to AWS') {
             steps {
                withAWS(region:'us-west-2') {
                    s3Upload(pathStyleAccessEnabled: true, payloadSigningEnabled: true, file:'index.html', bucket:'hantzyy')
                }
             }
        }
    }
}
