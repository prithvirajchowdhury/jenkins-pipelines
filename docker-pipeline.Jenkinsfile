pipeline {
    agent any

    stages {
        stage('portainer') {
            steps {
                deployPortainer()
            }
        }
    }
}
def deployPortainer(){
    sh "docker run -d -p 9000:9000 -v /var/run/docker.sock:/var/run/docker.sock portainer/portainer"
}
