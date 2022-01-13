node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'DockerHub') {

        def customImage = docker.build("eanene/My-NodeJs-Web-App")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}