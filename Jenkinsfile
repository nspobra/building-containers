node {
    checkout scm

    def customImage = docker.build("my-image:${env.BUILD_ID}")

    customImage.inside {
        sh 'node --version'
    }
    customImage.push()
    customImage.push('latest')
 }
