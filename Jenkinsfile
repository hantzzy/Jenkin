pipeline {
    agent any
    stages {
       stage('Build') {
             steps {
                sh 'echo "Hello World"'
                 sh  ''' 
                    echo "Muliline shell steps works too"
                    ls -lah
                 '''
             }
        }
    }
}
