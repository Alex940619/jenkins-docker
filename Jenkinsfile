node {

    checkout scm
    
    docker.withRegistry('https://registry.hub.docker.com', 'DockerHub') {
        docker login -u alex940619
        def customImage = docker.build("alexton/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
