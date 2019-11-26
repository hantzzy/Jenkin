pipeline {
    agent any
    stages {
       stage('Upload to AWS') {
             steps {
                withAWS(credentials:'IDofAwsCredentials') {
                    s3Upload(pathStyleAccessEnabled: true, payloadSigningEnabled: true, file:'index.html', bucket:'hantzyy')
                }
             }
        }
    }
}
