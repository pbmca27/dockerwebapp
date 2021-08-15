node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'DockerHub') {

        def customImage = docker.build("233723/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
