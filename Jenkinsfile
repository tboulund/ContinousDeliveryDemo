pipeline {
    agent any
    stages {
        stage("Deliver") {
            sh "docker build . -t my-website"
            sh "docker run -it --rm -d -p 87:80 --name web webserver"
        }
    }
}