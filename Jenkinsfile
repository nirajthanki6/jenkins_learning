pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello World"'
                sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                '''
            }
        }
            stage('BuildMore'){
            steps{
                input message: "Shall we build more?"
                sh '''
                echo "We are approved; continue!"
                ls -lah
                '''
            }
        }
    }
}
