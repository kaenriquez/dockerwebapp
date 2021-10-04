
node {
    checkout scm

    docker.withRegistry('https://hub.docker.com/', 'dockerhub.id') {

        def customImage = docker.build("miltonc/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
