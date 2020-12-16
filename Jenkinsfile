pipeline {
    agent any
    stages {
        stage("Deliver") {
            steps {
                sh "docker build . -t webserver"
                sh "docker run -it --rm -d -p 87:80 --name web webserver"
            }
        }
    }
}