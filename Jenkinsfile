node {

    checkout scm
    docker login -u alex940619
    docker.withRegistry('https://registry.hub.docker.com', 'DockerHub') {

        def customImage = docker.build("alexton/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
