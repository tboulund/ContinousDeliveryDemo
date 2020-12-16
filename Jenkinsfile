pipeline {
    agent any
    stages {
        stage("Deliver") {
            steps {
                sh "docker build . -t webserver"
                sh "docker run -it --rm -d -p 80:80 --name web webserver"
            }
        }
    }
}